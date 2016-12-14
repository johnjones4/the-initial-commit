---
layout: post
title: "Minko Gechev"
seo_title: "An Interview With Minko Gechev"
description: "I maintain quite a few projects at the moment; two of them which got quite popular recently are angular-seed and codelyzer."
links:
  - name: github.com/mgechev
    url: https://github.com/mgechev
  - name: blog.mgechev.com
    url: http://blog.mgechev.com/
projects:
  - name: angular-seed
    link: https://github.com/mgechev/angular-seed
  - name: codelyzer
    link: https://github.com/mgechev/codelyzer
tags: ["angular", "javascript"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain quite a few projects at the moment; two of them which got quite popular recently are [angular-seed](https://github.com/mgechev/angular-seed) and [codelyzer](https://github.com/mgechev/codelyzer).

Angular Seed is a starter for Angular 2 projects with statically typed, modular build system. I started it in early 2015 in order to give Angular 2 a try. I released it open source because there weren't many reliable starters at this time and there were a lot of people willing to see what Angular offers.

I'm one of the original co-authors of the official Angular style guide. While working on it, I was thinking how we can simplify and automate the process of enforcement of best practices listed there so I developed codelyzer. It's a tool for static code analysis of Angular projects which makes sure given codebase is aligned to the style guide to some extent. Codelyzer is something like eslint or tslint but on a higher level of abstraction, analyzing TypeScript code, components templates and styles. Having both Angular and the style guide being open source, it was natural choice to open source codelyzer as well.

A few other projects that I maintain are aspect.js - a library for aspect-oriented programming with JavaScript and TypeScript, a couple of utility libraries, UI components, contributing to Angular core and the mobile toolkit.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Angular Seed was mostly built to solve a problem that I had. I wanted a reliable starter that helps me to try Angular. Later I started working on "Switching to Angular 2" where I used the seed for the examples that I developed for the book. In the mean time I started a couple of other projects with Angular Seed. This helped me to find some of the flaws in the seed and fix them.

In contrast, when I built codelyzer I was thinking of how we can improve our development process with Angular. Everyone knows how annoying code reviews can be, especially when one of their goals is enforcement of common style. Codelyzer can *help* at least with this.

Finally, I developed aspect.js because for long time I've been missing a declarative library for aspect-oriented programming in JavaScript. After TC39 had a proposal for decorators and TypeScript introduced them into the language, I developed aspect.js. Currently I'm using it in a few of my projects.

### How has the project evolved since you first got involved or first released it?

Angular Seed evolved dramatically. Initially it contained a simple gulp script for the entire build process. Now the build is completely modular and statically typed. We have a level of abstraction on top of gulp which makes the project independent from the task runner. I really love how we introduced a separation between built-in tasks and project-specific ones. This allows easy way to override specific steps of the build pipeline and replace them with custom ones which also makes the process of upgrade to the latest version of Angular Seed quite easy. The build system now performs dozens of optimizations in order to produce the most efficient bundle possible.

Regarding codelyzer, so far there aren't any dramatic changes there except a number of incremental improvements; for instance, support for inline templates, later inline styles and since the last release external templates and styles. Probably next year the project will start getting more mature and we'll have to consider how to make the error reporting mechanism more robust, improve the performance, etc. That's when I expect the project to evolve more.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

In Angular Seed I got a lot of help from the community. Ludovic Henin helped a lot with making the project what it is today. I believe the seed is also more natural choice for making a contribution to. A lot of people are heavily relying on it every day for building their own products. They face different problems and opportunities to improve of the build process so I get a lot of feature and pull requests. In this project I spend half of my time in development and half in reviewing pull requests and issues.

On the other hand, codelyzer is more like a black box. It's a tool which builds an abstract representation of your Angular application and analyzes a bunch of abstract syntax trees (TypeScript, template, CSS and Angular expressions). There is one more active contributor in this project who helps a lot. For codelyzer I'd say that I spend about 90% of my time in development.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I had the chance to meet some amazing people over the years thanks to open source. In the Angular community you can see really well engineered software, starting from the Angular core so you can learn a lot. I appreciate the impact of Google on this. Another favorite thing is the fact that a lot of people are willing to improve already existing software in a very constructive manner - either firing issues with suggestions or opening pull requests.

On the other hand, sometimes there is lot of negativity and non-constructive criticism.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

There a couple of things which keep me involved. First, they solve real problems that people face on daily basis. Working on them, getting feedback, and exchanging ideas, I'm able to improve myself as a software engineer. Also, maintaining projects that are being used by tens of thousands developers around the globe helps me to think a little bit more conservative when introducing new features. I believe this is an important quality. Finally, I love coming up with abstract theoretical ideas and solving practical problems with them; this gives me a lot of possible improvements as part of the projects' backlogs.

### What is the most important thing someone submitting an issue or patch should know?

For an issues it's very helpful if people are following the project's guidelines and searching for similar problems before opening one. GitHub helps with the issue templates but still a lot of people are ignoring them. For patches I'd say, that if someone is willing to introduce a new feature into an open source project, it's first best to discuss the idea with the core maintainers. I really hate closing pull requests but sometimes they are too much out of the scope a project.

### What’s your development environment right now?

For the past a couple of years I've been using vim with tmux and iterm 2 on macOS.

### What was your first development environment? Do you miss anything from it?

In high school for about a year I was using Notepad on Windows. From time to time, especially when solving algorithmic problems I'm still switching to a text editor without syntax highlighting, and disabled semantic and syntax checking. It definitely decreases productivity but in the same time helps me get more concentrated, careful and think more about the code that I'm writing.

### Where do you see the open source software community headed?

I have better insight for the JavaScript community, so I'll talk about it. In terms of paradigm shift, for the last a couple of years developers are empowering the functional paradigm a lot. Now, after the final release of rxjs, we probably will see a lot of functional-reactive programming.

In larger scale, I see more and more high-quality open source projects being released by big companies. This has a lot of positives for developers because usually the code is well tested, documented and maintained. On the other hand, I see a strong centralization.
