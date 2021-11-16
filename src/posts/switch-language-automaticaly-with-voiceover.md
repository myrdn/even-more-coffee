---
layout: layouts/post.njk
title: Switch language automatically with VoiceOver
date: 2021-11-16T16:29:05.612Z
tags:
  - a11y
  - screenreader
---
I started using VoiceOver as my default screen reader on macOS Monterey to test manually websites I make. I use english as my default language but as I am french I often deal with french websites. 

One thing you should do when coding a website is to fill the `lang` attribute on your html elements to let assistive technology know what language it is dealing with. 

I was expecting that once I added french voice to VoiceOver it would automatically switch to french when I land on a page with `lang=fr` attribute. But it was not so here is the way to setup VoiceOver to automaticaly switch to voices you added with the VoiceOver utility :

1. Launch VoiceOver with cmd + F5
2. Enter the VoiceRotor with VO + cmd + shift + left/right keys
3. Select *Automaticaly select based on language*

You can now visit a website in your alternative language and if the correct attribute is filled VoiceOver will automatically switch to this language while reading the content.