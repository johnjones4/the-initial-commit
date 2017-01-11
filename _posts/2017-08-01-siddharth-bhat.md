---
layout: post
title: "Siddharth Bhat"
seo_title: "An Interview With Siddharth Bhat"
description: "The last thing I released was teleport, which was a CLI app written specifically to teach how to build \"useful\" things in Haskell."
links:
  - name: github.com/bollu
    url: https://github.com/bollu
projects:
  - name: teleport
    link: http://bollu.github.io/teleport
  - name: graph-reduction
    link: https://github.com/bollu/graph-reuduction
tags: ["haskell","python"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

The last thing I released was [teleport](http://bollu.github.io/teleport),
which was a CLI app written specifically to teach how to build "useful"
things in Haskell. When I started learning Haskell, I found it hard to learn
how to put things together, which was why I wrote the tutorial. A lot of
people seemed to like it, which I'm happy about :)

Right now, I'm writing [graph-reduction](https://github.com/bollu/graph-reuduction),
an implementation of a lazy functional language using a technique called
"graph reduction". There aren't very many references on this, so I plan on
writing a series of tutorials from the codebase. The only reference that exists
is [Implementing Functional languages, a tutorial](http://research.microsoft.com/en-us/um/people/simonpj/Papers/pj-lester-book/)
and a couple of related papers.

I also need to experiment more with [Reality Check](https://github.com/bollu/SublimeRealityCheck/blob/master/README.md),
a Sublime Text plugin for feedback-as-you-type with Python. I have a couple of
ideas, but I'm not sure in which direction I want to take it.

I'm maintaining the [Haskell bindings to Symengine](https://github.com/bollu/symengine.hs/),
but this has taken somewhat of a back seat the past couple of weeks since
college just started.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

They were mostly for issues that I wanted to solve. Sometimes, I wrote things
purely to teach people. Others were to fix workflows, libraries I wanted, etc.

### How has the project evolved since you first got involved or first released it?

Some of the older projects I used to contribute to, such as [PPSSPP](http://github.com/hrydgard/PPSSPP),
are doing splendidly. Others, like [VisPy](http://github.com/vispy/vispy), are
in a little bit of a slump due to the personal lives of everyone involved.

I think that is quite natural. Some projects hit critical mass and succeed,
others slowly fade away; most of the time, due to reasons not entirely in our
control.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend most of my time writing documentation and taking care of issues
and PRs.

Code is quite easy to write, but maintaining is a whole different ball game.
I try to rotate between projects that I'm working on so I don't burn myself
out.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I love the communities I particpate in in general, and how positive the people are. The Haskell
community in particular has some of the most wonderful people I've ever met.

The X-factor of the Haskell community, as I see it, is the confluence of
both super academic and super practical people, who work in tandem to
create really elegant solutions.

My least favourite is maybe the _perceived_ ivory-tower-ness of the community.
I think it's a difference in culture, but it needs to be bridged somehow.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I build things that I like and I use, so I see myself keeping them
updated as long as I'm around. For some of my projects, I wound up
sunsetting them and disbanding the team, since I couldn't find anyone to maintain them. For
larger projects, it's okay to make nice PRs and then drop off the radar as life
takes over.

I try to keep the [Bus factor](https://en.wikipedia.org/wiki/Bus_factor) of
anything I'm working on greater than 1.

### What is the most important thing someone submitting an issue or patch should know?

The fact that the person on the other end is a real person, and some kindness
goes a long way. Other than that, a descriptive patch / issue is always
appreciated over "bug, please fix".

### What’s your development environment right now?

I'm on Mac OS mavericks. I use Vim, Sublime Text, and emacs as text editors
depending on what I'm doing.

I do occasionally go back to Arch Linux on my desktop as I love the philosophy!

### What was your first development environment? Do you miss anything from it?

My first "dev environment" as a kid was LOGO on Windows 95, as taught by dad :)
First proper development environment was Visual C++. I don't miss much, but I
do miss the amazing debugging capabilities from time to time.

Though this isn't strictly dev environment related, I miss my
_childhood_ environment of being a kid and having all the free time in the world!

### Where do you see the open source software community headed?

That's a tough one! I see people moving non-code oriented media to the
open source model of collaboration since it has been hugey successful for
code. It's already happening with books like the [Homotopy type theory](https://github.com/HoTT/book) book.
Mathematicians are collaborating on the [polymath project](http://michaelnielsen.org/polymath1/index.php?title=Main_Page).

I think the main take away will be the "open source methodology" which I find
super exciting. Computing is a young field, and it's nice to see it influence
other fields that are far older and more established. I hope this
leads to richer interplay and sharing between these sciences.
