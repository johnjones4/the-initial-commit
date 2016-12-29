---
layout: post
title: "Mathias Bynens"
description: "Back in 2010, there was no easy way to reliably measure the performance of two or more pieces of JavaScript code, let alone compare those results across browsers."
seo_title: "An Interview With jsPerf's Mathias Bynens"
image: "mathiasbynens.jpg"
links:
  - name: mathiasbynens.be
    url: https://mathiasbynens.be
  - name: github.com/mathiasbynens
    url: https://github.com/mathiasbynens
projects:
  - name: jsPerf
    link: https://jsperf.com/
  - name: Benchmark.js
    link: https://benchmarkjs.com/
  - name: HTML5 Boilerplate
    link: https://html5boilerplate.com/
tags: ["html5", "javascript"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

Back in 2010, there was no easy way to reliably measure the performance of two
or more pieces of JavaScript code, let alone compare those results across
browsers. In an attempt to solve that problem, I created my first two
open-source projects: [jsPerf](https://jsperf.com/) (an online JavaScript
performance testing sandbox) and [Benchmark.js](https://benchmarkjs.com/) (the
JavaScript library used for the actual benchmarking on jsPerf).

Around the same time I started contributing to
[HTML5 Boilerplate](https://html5boilerplate.com/), which is a collection of
best practices and safe defaults for front-end projects built using HTML, CSS,
and JavaScript.

Later, I open-sourced [my dotfiles](https://github.com/mathiasbynens/dotfiles).
Along with the usual configuration files (`.bash_prompt`, `.bash_profile`,
`.vimrc`, and so on) I also automate my macOS system preferences, mostly through
the use of `defaults` commands. As such, I suppose
[the `.macos` file](https://github.com/mathiasbynens/dotfiles/blob/master/.macos)
is the most interesting part of my dotfiles repository.

In 2014, I started to open-source my
[walkthroughs of security CTF challenges](https://github.com/ctfs/write-ups-2014).

More recently, I’ve been creating open-source JavaScript modules that solve
various problems I run into.
[A lot of them](https://github.com/mathiasbynens?tab=repositories&q=unicode)
involve iñtërnâtiônàlizætiøn somehow — they make it easier for developers to
support non-ASCII Unicode symbols everywhere.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

As mentioned, jsPerf solved a very generic problem. Over the years, jsPerf test
cases resulted in performance improvements in various popular JavaScript
libraries such as jQuery, Backbone, and lodash, as well as optimizations in web
browser’s JavaScript engines. Everybody wins!

The reason for sharing my CTF walkthroughs was entirely different. In the
security community, there’s lots of smart people who can solve nearly any CTF
challenge. However, it seemed like not many among those take the time to share
their knowledge (which is understandable given the competitive aspect of CTFs).
As a newcomer to the security scene, I wanted to share what I learned with as
many people as possible.

### How has the project evolved since you first got involved or first released it?

HTML5 Boilerplate soon had a diverse community of active contributors, and
became hugely popular. It’s weird to see your contributions to an open-source
project reflected in the HTML source code of websites like Google, Microsoft,
and NASA.

The CTFs organization on GitHub that once started out with just me sharing my
write-ups, now has 20 committers, and multiple active repositories. It’s been a
while since I contributed, which makes it all the more lovely to see how the
community keeps the project going. It’s become an excellent resource for anyone
interested in security, regardless of their skill level.

The initial version of jsPerf was hastily written in PHP. Last year, keeping
jsPerf running became too time-consuming, and I was forced to take down the
website. I promised to bring it back online once the codebase was rewritten from
scratch in Node.js. Immediately, some open-source community members started to
work on that, and recently jsPerf v2 went live!

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I don’t really have a fixed schedule here. 😳 I get email notifications for
every new issue or comment on my projects. Whenever I can respond or fix the
problem quickly, I do so. But if the issue requires more consideration, it has
to wait until I find time to deal with it properly, which can take
`rand(0, Infinity)` seconds.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Take [my dotfiles repository](https://github.com/mathiasbynens/dotfiles) as an
example. Before I open-sourced my macOS configuration scripts, I had to figure
out most of those commands on my own. Now that the project has gotten a bit of
exposure, it’s gotten to the point where contributors regularly suggest commands
for new system settings I’ve never even heard about! What started out as me
sharing the tricks I found out about has turned into people sharing their nifty
discoveries with me.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I try not to start a new project unless I have a use for it myself.

Since most of my projects were created to solve a problem I was having, it makes
sense for me to continue maintaining them — at least until the problem is no
longer relevant.

### What is the most important thing someone submitting an issue or patch should know?

Search the README, docs, and issue tracker before filing a new ticket or
submitting a patch. When filing a bug, include a minimal test case that
reproduces the problem. Follow the existing coding style. Err on the side of
over-communication.

### What’s your development environment right now?

OS-wise, I’m most productive on macOS. My terminal emulator of choice is iTerm2,
although I’m keeping a close eye on HyperTerm.

As for my text editor: I keep hopping back and forth between Sublime Text (for
longer coding sessions) and Vim (mostly for quick edits).

### What was your first development environment? Do you miss anything from it?

My very first Development Environment™ was Windows 95’s Notepad.exe, paired with
CuteFTP to publish files to a website. Let’s just say I don’t miss it.

### Where do you see the open source software community headed?

Lately more and more big corporations have started to embrace open-source. I
think (and hope) that trend continues in the future.
