---
layout: post
title:  "Tom MacWright"
description: "The projects I spend most of my time on are documentation.js, simple-statistics, and big."
links:
  - name: www.macwright.org
    url: http://www.macwright.org/
  - name: github.com/tmcw
    url: https://github.com/tmcw
projects:
  - name: Documentation.js
    link: http://documentation.js.org/
  - name: Simple-Statistics
    link: http://simplestatistics.org/
  - name: Big
    link: http://www.macwright.org/big/
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

The projects I spend most of my time on are documentation.js, simple-statistics,
and big. There's a long tail of probably around 50 smaller modules that are
still maintained and used, but those are the big ones that are mostly free-time
commitments. Within work at Mapbox, I maintain Turf, Mapbox.js, toGeoJSON,
and another long tail of other stuff.

Most projects come from some personal need - I wanted to make presentations,
wanted to create documentation, and so on - and then there needs to be something
that I can learn from making the thing. For documentation.js, that was learning
about Abstract Syntax Trees for JavaScript. They're an awesome abstraction and
the fundamental thing that makes documentation.js possible. I wrote
simple-statistics to test the idea of literate programming and to learn
statistics.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I try not to create projects that I don't have a use for. simple-statistics is
probably the furthest on the border - the basic statistics I use but some of the
complex functionality was fun to write but not personally useful.

And, yeah, you have to think about opportunity, roughly in the same lens as
companies think about addressable markets. How many people have this need, and
how big could it grow? How general is the problem? Really successful projects
solve really general problems.

### How has the project evolved since you first got involved or first released it?

On one hand, there's big - a presentation system that I wrote in 2012. Over the
years it has changed almost not at all, and I see no reason to change it. It's
an extremely simple answer to very well-defined problem.

On the other, documentation.js changes rapidly. We started with a
streams-oriented approach, and then switched entirely to a functional approach.
It started with one kind of templates, and ended with a totally different one.
The problem space it attacks is large and not very well-defined, so there are
lots of things we could build and they'd get the job done.

I'd love for all projects to have lots of clarity of focus, but usually they end
up reflecting the problems they try to fix. Some of those problems are hard, and
others are intractable.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

Probably too much. I've definitely shifted from trying to spend lots of time
doing development to lots of time building the community - that means writing
longer and more thoughtful responses to people's questions, doing more support,
making sure that PRs get merged on a reasonable schedule. On top of a typical
9-6 work schedule, open source projects consume maybe 10 hours a week.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The communities really vary, depending on what you're building. The community
around a technical project with a steep learning curve is often the easiest kind
to hang out in: you get fewer drive-by support requests, and more people with
well-developed question-asking skills.

I think documentation.js has been doing well in terms of building a group of
people who contribute, and a lot of the best ideas in the project have come from
the outside. But getting work done and achieving goals are kind of different
things and we're only starting on the second - how do you organize these chunks
of work into releases? It's tricky to make the parts that require opinion and
decision-making work.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I stay involved as long as I feel like something is useful - whether to the
larger community or to myself as a learning opportunity. When things start being
thankless, or a project is unsuccessful, I'll let it go - earlier this year I
put 40 projects up for adoption [http://www.macwright.org/2016/01/30/adopt.html](http://www.macwright.org/2016/01/30/adopt.html).

### What is the most important thing someone submitting an issue or patch should know?

The importance of communication. Everyone spends so much time asking follow-up
questions and trying to get the gist of what a PR is about. You'll occasionally
see seasoned contributors really describe a change in detail, and it's amazing.
So, overcommunicate and think hard about what the other person knows and doesn't
know - how much context do you need to unpack?

### What’s your development environment right now?

I use neovim, a somewhat improved version of vim, and run it within iTerm, and
run zsh. My neovim setup is relatively simple - no "folder drawer", I find
everything by searching, no fancy status line or whatever. This all runs inside
of OSX, and there again I remove a lot of stuff - Bartender lets me hide menu
bar icons, I turn off the system clock to remove that distraction, and turn off
transparency. And OSX runs inside of a two-year-old MacBook Pro, which I'll
update the moment that Apple releases the new one.

### What was your first development environment? Do you miss anything from it?

This is way back, but I used jEdit all the time, and ran it on a Motorola clone
of a Macintosh, available briefly between 1995 and 1997. jEdit had a plugin that
would save directly to FTP, which was how I updated websites.

I don't miss anything about the technology, but the visual style of Mac OS 9 was
the peak of computing aesthetic.

### Where do you see the open source software community headed?

We're in a weird spot, right now. I have one foot in the corporate open source
world - Mapbox's software is mostly open source and I work on it 9-6 - and one
in the enthusiast world, which is where documentation.js and simple-statistics
come from.

More and more projects that I'm seeing come from people who do them as part of
their jobs, at companies. Which is great, that it's mainstreamed enough that
companies do it, but also it's increasingly awkward for companies to interact
with each other and with enthusiasts. How do you balance the concerns of
contributors who have an hour or two to contribute, versus folks who are paid
well to do similar tasks on a regular basis?

Governance and licensing both have been in a very laissez-faire mode for the
last 5 or more years: BSD and MIT licenses rule most new software, and while we
have CoCs more often, projects don't have the organizational structure of, for
instance, Apache or Linux. I don't see much movement on the licensing front,
but I do think that organizational structure will start to see some CoC-like
reusable text and common tricks emerge, so that projects can deal with the
sometimes overwhelmingly town-hall-like discourse of GitHub.
