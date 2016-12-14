---
layout: post
title: "Daniel Stenberg"
seo_title: "An Interview With cURL's Daniel Stenberg"
description: "My primary project is curl."
image: danielstenberg.jpg
links:
  - name: daniel.haxx.se
    url: https://daniel.haxx.se
  - name: github.com/bagder
    url: https://github.com/bagder
projects:
  - name: cURL
    link: https://curl.haxx.se/
  - name: c-ares
    link: https://c-ares.haxx.se/
  - name: libssh2
    link: https://www.libssh2.org/
tags: ["curl"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

That's actually a harder question than it may sound.

My primary project is curl. I also maintain a few projects that I'm still
fairly active in, like c-ares and libssh2 and I have two book projects that I
also maintain ("http2 explained" and "Everything curl"). But even after those,
there's a whole slew of dormant or mostly abandoned projects that I
occasionally spend some time and energy on.

Just about all open source work I do on spare time originate in a personal
need or desire to get something done. An itch I had to scratch if you will.
And once the thing has been released in the wild as open source and it catches
some speed and traction, I stick around and work on it.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

In the curl case, it was started a very long time ago when I wanted to write a
tool for getting currency rates from a HTTP server. That basic little program
for a single task then grew to become something much bigger and powerful over
the years. A lot of my other projects have then later sprung up to help me
improve curl in various aspects. My work on both c-ares and libssh2 for
example, have been motivated by that.

I'm not a "grand visionary" or forecaster who makes things that I think
someone might need in a future. I write tools and libraries that we need now
to perform basic tasks. Mostly after I've identified areas that aren't covered
or are served badly by the existing projects. And then I keep iterating and
improving until the end of days.

### How has the project evolved since you first got involved or first released it?

The first version of curl was released in 1998 and was just a few hundred
lines of code written by me and a handful of contributors. curl of today is in
total, when also including test infrastructure, over 200,000 lines of code and
we have well over a hundred contributors per year. Our THANKS document lists
almost 1500 names of persons who have contributed during the project's life
time.

We started out as a small tool with a very limited feature set. Now we have
almost 190 command line options, support for 20 something protocols, we also
ship a library and we estimate that curl code is used (directly or indirectly)
daily by every human in the connected world! So yes, the project has truly
exploded in terms of contributors and use and is a few magnitudes larger in
code size compared to the first version.

In other ways it hasn't changed much. We're still, 18 years in, a fairly small
project lead by me, primarily maintained and worked on by spare time
developers and we still keep most of the discussions on mailing lists. I still
know most of the code. I still spend my evenings and nights debugging, writing
email and developing curl. It is still a lot of fun.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I'm allowed by my employer (Mozilla) to spend parts of my work hours on curl,
but apart from that I mostly continue a routine I established a long time ago:
when the rest of my family goes to sleep, I get a couple of hours of curl/open
source work done. That's usually around 22:00 to 01:00 or so. When the house
is silent and dark, I get stuff done. Well, at least that's the general plan.
Some nights I'm just too tired to actually pull it off.

As a maintainer of the project, I get far too little actual developing done
and a big share of my curl time is spent triaging, debugging, reviewing and
supporting others on mailing lists and issue trackers. I also spend time on
writing documentation and I run, edit and admin the web site which also
requires some level of attention.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

My projects are usually written in portable C and are tools/libraries used as
building blocks others can build upon. I think that brings in and attracts a
certain kind of people, usually of the older type and the ones who are already
fairly technical and usually experienced.

A good part of our community is that we have very few trolls or hostile people
around and we've never had a problem with attitudes or bad behaviors. Many
good friends really!

Bad parts would probably include our lack of diversity - we're mostly western
white old males, and that I find it very hard to grow our developer base. I'm
of course aware that we share these problems with many other projects.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I participate in my open source projects to a small part because of a feeling
of obligation, but the major driver is the shear joy. I like building stuff
that people can use to accomplish things. I like feeling that I bring tiny
pieces to "society" that makes it better and helps make cooler products,
devices and tools. And when I've shipped something that people like and use, I
want to stick around and fix the bugs I included so that my stuff actually
works as intended!

The feedback loop, when people say thanks and express gratitude can make me go
very far and put in a lot of effort.

Open source development is my primary and greatest hobby.

My long term plans for all projects I maintain is to engage more developers,
spread the knowledge, spread the responsibilities, try to get more people
interested and try to make decisions into a team thing and not done benevolent
dictator style. So that I can become just one of the team and the project can
move along without me having to steer much. I must admit this isn't succeeding
everywhere.

### What is the most important thing someone submitting an issue or patch should know?

Two things:

A) there's no such thing as a too small patch or issue. Every little bit
counts and it is way better if people fix tiny problems rather than just
sitting around waiting for someone else to do it. Also, small fixes and
patches are just perfect to get warmed up with and get familiar with the
project, its code and its community. Don't wait, just dive in. And a fix
doesn't have to be code, it can just as well be documentation or polishing up
the web site.

B) try not to get intimidated by "leaders" or apparently "experienced" people
in projects. We all started out without knowing everything (and a lot of us
aren't that know-it-all as it may appear to the audience). We can all
contribute and help, no matter experience levels. Actually, it even helps to
bring different viewpoints to projects and since there will always be
newcomers, getting a newcomers view and input into the project is also good.

I suppose both those could be put into a single short and sweet phrase: "don't
hold back"

### What’s your development environment right now?

My development environment hasn't changed much the last decade. I'm a Linux
guy so I use a fairly performant Linux desktop at home, with two screens. I
prefer Debian Linux so that is what I use, and I edit all source code with
emacs - which I've learned tells people a lot about my age! =) I have a set of
other machines too, like a laptop for when I travel/speak, a mac for doing Mac
tests, a dedicated video conference laptop etc but they're not the ones I ever
use 12 hours straight to develop on.

### What was your first development environment? Do you miss anything from it?

I first learned to code Basic back in 1984 on a Commodore 64. No, there's
really nothing to miss about that, even if I of course had an awesome time
with that "bread box" and it gave me the entry point to where I am today.

I "discovered" unix-like systems in 1991 when I worked for IBM and I've been a
"command line cowboy" ever since and Linux has been my prefered OS since well
over fifteen years.

I'm not a nostalgic person. I tend to not get stuck in the past or think of
certain moments in history as the good old days. I like current technology and
I want to see what's next. I want to develop what's coming. The best
development environment is what I have right now. And it can only get better!

### Where do you see the open source software community headed?

Bigger, brighter, faster.

I think we've still only seen the early days of open source growth. I think
we'll see an even greater share of software in general switch to open source
going forward. To allow companies to iterate faster and sell the next
generation of devices earlier, and to allow said companies to easier change
platforms between generations. To be able to collaboratively improve things,
like operating system kernels or server engines. Where there's no real need
for differentiation commercially, companies will continue to gain to switch to
open source and I think we will see the proprietary systems develop to more
and more become layers on top of open source building blocks.

And the more companies use open source, the more they will provide code back
and help populate the open source communities and projects.
