---
layout: layouts/post.njk
title: Reveal encrypted email address with echo and sed
date: 2021-09-17T17:24:20.003Z
tags:
  - Javascript
  - Email
  - Unix
---
Here is a stupid tool I wrote to hide your email address while sharing it on internet.

It is pure client-side javascript, using simple substitution cryptography. It generates a command with common unix utilities `echo` and `sed`. You just need to enter your email address and you'll get the command. You can share the generated command on your website, your visitors will need to paste it into their terminal emulator and it will reveal the email address.

Here is the output for my email adress :

`echo 'ʢяʃЖʖʡ@ʢʥʃ1ζɑʥЮЮ11λʡ1ʄ' | sed 'y/яʃЖʢʖʡ@ʥɑ1λʄЮζ/yrdmin@oce.tf-/'`

I understand nobody will use it because who wants to open a terminal before sending an email ?

*But it was fun to do.*

You can find the tool [on this website](https://myrdn.github.io/mail-address-encryption/)