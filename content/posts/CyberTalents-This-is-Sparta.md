+++ 
draft = false
date = 2022-07-03T22:15:46+01:00
title = "CyberTalents - This is Sparta"
description = ""
slug = ""
authors = ["Rxfa"]
tags = ["CyberTalents","Web","Easy"]
categories = ["Writeups"]
externalLink = ""
series = []
+++
 

Room: https://cybertalents.com/challenges/web/this-is-sparta

Difficulty: Easy
# Let's get started

![Login Page](/9741a53dea7549bb803e3201ba03b7c0.png)

This is the first thing we see after starting the challenge, we try a few different common usernames and passwords with no success, so we go take a look at the page source and find two scripts at the end of the page.

![Page Source](/074067308735c0290kh8ggt8.png)

The first is easy to understand, it's the hint and now we've all (accidentally) read it, the other one is not as straightforward and to be honest, it just looks like gibberish. What we see in the second script is [obfuscated](https://en.wikipedia.org/wiki/Obfuscation_(software)) code, that is, code that went through a series of transformations made with the intent of making the code harder to understand ([security through obscurity](https://en.wikipedia.org/wiki/Security_through_obscurity)) in order to prevent tampering and deter reverse engineering. 

Fortunately for us, it's a really small script so we shouldn't find much trouble trying to deobfuscate it, we head to https://beautifier.io/,  paste all the obfuscated code and hit enter.

![deobfuscated code](/962f46a5d81645918d3794db56a7f43d.png)

Good.

Now we try to login with the credentials we just got.

![flag](/1886f31586a941a3bb0032cf18f7be74.png)

And I guess we're done here.

Make sure to give me a follow on my GitHub and feel free to contact me on Discord.

Github -> https://github.com/Rxfa

Discord -> Rxfa#9148