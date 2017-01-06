---
layout: post
title: "Jason Wolfe"
seo_title: "An Interview With Clojure Developer Jason Wolfe"
description: "I'm the primary author and maintainer of several open-source Clojure projects, including schema, plumbing & graph, fnhouse, hiphip."
links:
  - name: github.com/w01fe
    url: https://github.com/w01fe
projects:
  - name: schema
    link: https://github.com/plumatic/schema
  - name: plumbing & graph
    link: https://github.com/plumatic/plumbing
  - name: fnhouse
    link: https://github.com/plumatic/fnhouse
  - name: hiphip
    link: https://github.com/plumatic/hiphip
tags: ["clojure"]
---

###What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I'm the primary author and maintainer of several open-source Clojure projects, including [schema](https://github.com/plumatic/schema), [plumbing & graph](https://github.com/plumatic/plumbing), [fnhouse](https://github.com/plumatic/fnhouse), and [hiphip](https://github.com/plumatic/hiphip).   These projects all started as internal libraries at my former company, and were extracted and open-sourced both to aid in recruiting, and as a personal labor of love to try to give something back to the Clojure community.


###If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Typically, both.  As a small startup, most of our efforts necessarily went towards building functionality that would help us in the near-term.  But when considering what to open-source, we focused on the bigger ideas we thought would have the highest impact and utility to the community over a longer time scale.

For example, we started work on Schema to help address concrete issues around documentation and testing that we encountered as our engineering team grew.  However, even at the earliest stages of its design, we had our eyes on a bigger picture that would eventually include contracts, test data generation, and API tooling (inspired by similar projects for other programming languages).  


###How has the project evolved since you first got involved or first released it?

It varies.  Some projects, like [hiphip](https://github.com/plumatic/hiphip) (a primitive array manipulation library) haven't changed much since their initial release.  Others, such as Schema, have continually evolved to add functionality and features and keep up with changes to Clojure(Script) itself.

Schema is especially interesting in this respect, as the upcoming 1.9 release of Clojure includes a new component called [spec](http://clojure.org/about/spec) which aims to solve essentially the same set of problems.  While I'll continue to support Schema for the time being, I think it's served its purpose and look forward to the community coming together around `spec` once it's released.


###How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

When I'm developing on a new feature, I'll often focus exclusively on that until it's finished.  Otherwise, I usually try to respond to issues promptly when they are filed, and periodically knock out a batch of less-critical bugs and suggestions that have built up.


###How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Overall, I feel lucky to have the opportunity to be a part of such a great community.  I've worked closely with a few folks who have contributed big chunks of functionality, and also merged lots of smaller contributions that appeared out of the blue -- both of which have been great experiences.

The hardest part of maintaining a project for me is saying no.  When someone has an idea or puts up a PR that doesn't fit into my vision for a project, I first try to ask questions to learn more their ideas for how this functionality would be used and evolve.  Sometimes that changes my mind; and if not, I often suggest creating an extension library to work out the idea further, which we might consider incorporating down the road.


###What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

My new job doesn't use Clojure, so I haven't had much impetus for developing new features in these projects lately.  That said, maintaining them doesn't take much of my time, so I'm more than happy to keep them running so long as they're still generating significant value for the community.


###What is the most important thing someone submitting an issue or patch should know?

If you're submitting a bug report, please try hard to include a minimal test case.  It makes things so much easier for the maintainer (and sometimes you may even discover that the bug isn't, in the process).  

For substantial changes, please add an issue to discuss them first.  Making sure we're on the same page about the desirability and implementation strategy of a change before coding can save time (and potentially, hard feelings) for everyone involved.


###What’s your development environment right now?

I've always been an Emacs + Cider user for Clojure -- but lately I've been writing Scala using IntelliJ.   


###What was your first development environment? Do you miss anything from it?

I do miss some of the great features in SLIME for debugging Common Lisp programs.  But, to answer the question literally: while I do still have some nostalgia for GW-BASIC, I can't say I miss the line numbers.  


###Where do you see the open source software community headed?

I don't really feel qualified to make any big predictions.  That said, I think Github and other recently developed tools have largely helped the community become more open and inclusive, and I hope that trend continues.  
