---
layout: post
current: post
cover: /assets/images/cloud-services-cant-be-trusted-client-side.jpg
navigation: false
title: "Cloud Services Can’t be Trusted: Client-side Crypto to The Rescue"
date: 2013-07-26 10:18:00
tags: []
class: post-template
subclass: "post"
logo: assets/images/ghost.png
author: ghost
---

The era of trusting Google, Yahoo, Microsoft, whoever to keep your data and communications private is over. You just can’t trust the law, government, or cloud services to protect you. What you can trust is math. The only solution to true privacy in todays post patriot-act world is client-side cryptography. That is, your data and communication is encrypted on your machine in such a way that cloud services could not reveal your information even if they wanted to because you alone possess the key to its decryption. This not only protects users, it protects the companies that offer these services because they can truly say to government entities that they CAN’T hand over unencrypted user data.

This is, in fact, exactly what made it possible for Kim Dotcoms’ MegaUpload to be reborn as Mega. The encryption/decryption key is generated client-side ensuring that no one but yourself and people you wish to share with can view your files. Cloud services that wish to ensure their users privacy must employ similar methods because ‘trust’  just doesn’t cut it anymore. Security researcher Ruchna Nigam excellently describes the way Mega did this.

“All data present on the Mega servers is encrypted and so Mega never sees the content of your data. This can be easily verified since all encryption is done by open source, clear text client-side scripts. (DotCom was even confident enough of the strength of his encryption to announce a reward of 10,000 Euros to anyone who can break it) In short, the security of the data depends on the holder of the keys i.e. the user. This also works in their favour since they avoid copyright problems they had faced with Megaupload that led to it being taken down finally, but in the words Kim DotCom this is a small advantage compared to the freedom from surveillance they’re providing their users with.” - [http://bit.ly/18FB9Zr](https://href.li/?http://bit.ly/18FB9Zr)

![image](/assets/images/cloud.jpg)

Mega is not the first to try this (check out [securesha.re](https://href.li/?https://securesha.re/)) but they have significantly advanced the cause by creating [an SDK](https://href.li/?http://www.itnews.com.au/News/349529,mega-offers-free-client-side-crypto-sdk.aspx) that lets developers build on their platform without having to worry about the client-side cryptographic complexities involved. Or, if you’re a real cowboy, dig right into [crypto.js](https://href.li/?https://code.google.com/p/crypto-js/): A growing collection of standard and secure cryptographic algorithms implemented in JavaScript using best practices and patterns. See in detail [how securesha.re works](https://href.li/?http://blog.strml.net/2013/01/mega-was-second-announcing-first-client.html) and a [visual explanation](https://href.li/?http://blog.fortinet.com/Security Research/DotComs-Mega-Encryption-Scheme-Illustrated/) of Megas’ methods.

The real point I want to drive home is this. Trust is gone. The services are snooping. The government is snooping. Your employer is snooping. If you’re a cloud service who wants users trust, there is one option: Client-side encryption. Get at it.
