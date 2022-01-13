---
layout: post
current: post
cover: /assets/images/entropy-and-random-number-generators.jpg
navigation: false
title: "Entropy and Random Number Generators"
date: 2013-08-14 10:18:00
tags: []
class: post-template
subclass: "post"
logo: assets/images/ghost.png
author: ghost
---

This is a selection from a recent [Security Now podcas](https://href.li/?http://twit.tv/sn)t with Steve Gibson. I highly recommend listening to it.

Leo: Aren’t all algorithmically based random numbers pseudo?

Steve: No, because you can use physical properties of quantum physics.

Leo: So it’s using, like, chaos theory?

Steve: Yeah, it’s actually using - it’s using, for example, one of the actual random number generators is to reverse bias what’s called a “tunnel diode.” And there’s actual - if you put a reverse bias across the diode, it will not conduct. But every so often an electron that is being - there is a charge there, pulling the electrons across. But the diodeness prevents it. But every so often one goes through. But you never know when. It’s completely unpredictable. And so you could create then hardware around that tiny little bit of actual quantum physics to create completely unpredictable, true random numbers that will never repeat, that are not algorithm based. And Intel built that into the silicon from Sandy Bridge on.

Leo: Wow.

Steve: So it’s neat.

Steve: Well, sometimes there’s a problem, which is that the - oh, and the other cool thing about this is it is high bandwidth. And that’s key because there have been lowbandwidth random number generators. For example, you could use - turns out you can use the timing of the various clocks in the PC because there’s - there are phase-locked loops that synchronize crystal clocks in a PC, and there is noise generated that is also truly random. The problem is it’s not much. Many times, for example, a big server, which is really busy creating tons of SSL connections per second, it’s hungry for randomness. It’s consuming, like, the pool of randomness in the server at a high rate. So you need to be able to be adding more entropy at the rate that it’s being consumed by the way that the server’s operating. So what often happens, what often is done is that random numbers are used to seed pseudorandom number generators. So the PRNG, the pseudorandom number generator, is able to run at very high speed algorithmically, and then it’s constantly being reseeded at a lower bandwidth rate, but still enough that the entropy never drains out of the entropy pool in the pseudorandom number generator. Enough new entropy is trickling in to keep things completely unpredictable. Anyway, really smart guys have thought about this and figured out how to do it. It’s very cool stuff.
