---
layout: post
title: "Matteo Collina"
description: "I maintain more than 200 open source modules on NPM, plus I am a collaborator on Node.js itself in the streams working group."
image: "matteo.jpg"
links:
  - name: github.com/mcollina
    url: https://github.com/mcollina
  - name: www.matteocollina.com
    url: http://www.matteocollina.com/
projects:
  - name: Split2
    link: http://npm.im/split2
  - name: Cloneable-Readable
    link: https://www.npmjs.com/package/cloneable-readable
  - name: MQTT
    link: https://www.npmjs.com/package/mqtt
  - name: MOSCA
    link: https://www.npmjs.com/package/mosca
  - name: UpRing
    link: https://www.npmjs.com/package/upring
  - name: pino
    link: https://github.com/pinojs/pino
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain more than 200 open source modules on NPM, plus I am a collaborator on
Node.js itself in the streams working group. My OSS modules range from highly
downloaded utilities like http://npm.im/split2 and
https://www.npmjs.com/package/cloneable-readable to protocol libraries like
https://www.npmjs.com/package/mqtt or https://www.npmjs.com/package/mosca. I
recently developed https://www.npmjs.com/package/upring.  
At the beginning of this year, my colleague David Mark Clements and myself wrote
Pino, the fastest logger for Node.js (https://github.com/pinojs/pino). You can
see the full list at https://www.npmjs.com/~matteo.collina.

I create some of those because either myself, a colleague or a client (I am with
nearForm, a consulting firm in the OSS space) needed them.  

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Both. I did my Ph.D. in the Internet of Things (IoT) space, and I developed
Mosca as part of my thesis. In the process, I become the lead maintainer of
MQTT.js because Adam did not want to be involved. I develop a lot of “small
modules”, little things I can reuse across modules.

We developed Pino because during a consultancy engagement
(http://www.nearform.com/nodecrunch/client-case-study-net-a-porter/) we were
asked what logger we should recommend that had very little overhead. We tend to
scratch our own itch.   

### How has the project evolved since you first got involved or first released it?

Since 2013, when my first OSS project got some attention (LevelGraph, part of
the Level community, together with Julian), the download and adoption of my OSS
modules have grown significantly, up to 15 million downloads in 2016. My IoT
projects, MQTT.js and Mosca, have grown in usage, and MQTT.js is now used in the
SDK of AWS IoT, IBM Bluemix, and Azure IoT.

The first version of the Pino logger was in February, and its ecosystem has been
growing steadily since then. We have a third committer, James, who help us
developing the project.  

Node.js itself has been growing, both in adoption and as an organization. There
are more than 60 collaborators, and in fact I have been to the collaborator
summit right after Node.js Interactive in Asutin.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I do several things for my OSS projects, and I classify them in mainly three
categories: experimental, actively developed, and done. A project is “done” when
I consider it finished, and it serves the purpose for which I built it: for
these projects, I usually do not develop new features, but I rather review and
manage contributions. I code new ideas into experimental projects, and they
might see usage or not, depending if someone find them useful. Experimental
projects have most of my attention.

In general, I tend to divide my time equally into pursuing new ideas and
maintaining things that are being actively used. I tend to defer to the
community for bug fixing, and I review and accept PRs frequently. I also speak
at conferences very often about my OSS projects.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The community is why you get into OSS, and it is both invigorating and saddening
at the same time. In some ways, it’s like the startup life: a rollercoaster. One
day, someone tells me: “you changed my life, I am so much happier now”. Then,
some days after you receive an email “help me or I will lose my job”. People e
xpect you to be available, because you do OSS: I must choose if I can help that
guy, or stay with family.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I am currently paid (by nearForm) for maintaining most of my OSS projects,
MQTT.js and Mosca excluded. I keep contributing for all the people whom life I
can improve. The long term plan involves finding new lead maintainers for most
of my successful projects, do you want to help?

### What is the most important thing someone submitting an issue or patch should know?

There is a major difference between issues and patches. When opening an issue,
you should know that the author is making you a gift by responding. Do not
expect a quick response, and appreciate when there is one. Stop complaining. I
recently got some emails “please help me or I will lose my job”.

Submitting a patch is different, and it requires some grit: the authors are
going to reject it, mainly because it will cause added maintenance for them.
Keep going, and address all the objections the authors will report.  

### What’s your development environment right now?

I develop on a 2014 MacBook Pro 13’’ with i7, 16GB of RAM and 1TB SSD. I code
mostly using VIM and Tmux in the terminal. I use Docker for spinning up the
occasional database or infrastructure that I needed. I have an 24’’ external
LCD that I plug on when I am not traveling.

### What was your first development environment? Do you miss anything from it?

My first development environment was an Amiga 600. I miss playing good games on
it. Joking aside, the Vim+Tmux combo suits my needs completely.

### Where do you see the open source software community headed?

Companies like nearForm helps maintaining a lot of the OSS ecosystem. I see more
and more companies contributing back to the ecosystem and move things forward,
independently from tech giants.
