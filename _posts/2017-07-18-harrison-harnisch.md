---
layout: post
title: "Harrison Harnisch"
seo_title: "An Interview With Buffer's Harrison Harnisch"
description: "An Interview With Buffer's Harrison Harnisch"
links:
  - name: github.com/hharnisc
    url: https://github.com/hharnisc
projects:
  - name: Tabbie
    link: https://github.com/hharnisc/tabbie
  - name: hypercwd
    link: https://github.com/hharnisc/hypercwd
  - name: Python Meteor
    link: https://github.com/hharnisc/python-meteor
tags: ["javascript"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

Tabbie - A Chrome Extension That Helps You Manage Tabs

There was a period of time where I needed to context switch a couple times a day, and every time I did I either closed all Chrome tabs or minimized Chrome. In either case this lead to rebuilding all the context, or consuming 90% of the computer's memory. After searching around, there were a few existing solutions but they were either trying to do everything or designed for a different use case.

hypercwd - A plugin for Hyper terminal that allows opens new tabs in the same director as the current tab.

Hyper terminal was brand new at the time and the Zeit team had just implemented a basic plugin system. I had been using Hyper for a couple days and loved everything about it, except that new tabs always opened up in the home directory.

Python Meteor - A Python Client For Meteor

I was working at Apple at the time, building tools to automate the testing infrastructure. I wanted to use Meteor to control and visualize the system since it had most of the real time plumbing figured out. Most of the existing automation tools at Apple where written in Python, so I needed to find a way to bridge the gap. After trying a couple other Meteor Python clients, they all seemed to be incomplete or synchronous. So I created an asynchronous library and shared it.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

In each case, these projects were created to solve a specific problem. I had tried to find other solutions and then coded as a last resort.

The Tabbie project has been particularly interesting however, it's become pretty clear that there's a huge opportunity to improve the browser. Not so much the rendering engine itself, but the frame around it. We're still basically on the same feature set proposed in the early 90s with Mosaic and Netscape. I think it's one of the reasons which things like Electron exist, they give developers and users more control over the frame around the browser.

### How has the project evolved since you first got involved or first released it?

Tabbie - I released this project thinking it wouldn't get more than a few dozen downloads. But it quickly climbed to the thousands after a couple days. I've learned a ton about how people use and think about tabs and have used their feedback (review, issues and google analytics) to improve Tabbie. It's also become clear that I need to be more mindful of a11y features, so it's become a top goal to make this a tool for everyone.

hypercwd - As Hyper adoption increases, more issues and feature requests have been filed on Github. Especially for things like Windows and multiple tab support.

Python Meteor - This project has been pretty stable, and that's in part because the Meteor team did an awesome job spec'ing out the DDP protocol. There have been a few bug fixes from others here and there, but nothing major.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I aim to spend an hour per week contributing something to OSS. Sometimes it's focused on one project and other times it might be split between multiple project for smaller tasks.

Tabbie - Recently this has been the most involved project, there have been quite a few feature requests and a few bug fixes. Bug fixes tend to come in the form of pull requests and feature requests in the form of Github issues. I've been in development mode on this, and would not consider this project "feature complete".

hypercwd - This was pretty quiet for a while, mostly community management with a focus on keeping the project simple. There was a case where a feature request turned into someone creating another isolated plugin, which is really great! More recently, since adding support for Windows I've been in development mode on this project.

Python Meteor - Mostly just triaging issues as they come along.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The community around the projects seem to have a positive and collaborative atmosphere. I like to recognize and celebrate contributors because they're such an important part building software. It's amazing that we can solve problems like this together, and I think we live at a point in history where productivity is higher than it's ever been.

I'd love to see more diversity in the OSS community. We're the sum of our parts and if everyone brings in different skills and backgrounds, we get better and better over time.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

It's the people involved that keep me motivated. Once you release something into the world, other people start using it and even depend on it. I like to pick projects that solve problems I'm having because it aligns my personal needs with the needs of people depending on the project. This helps me determine how to spend my weekly OSS time and when to stop working on a project.

One of our goals at Buffer is a deeper commitment to OSS, so it's very likely I'll be spending more time contributing!

### What is the most important thing someone submitting an issue or patch should know?

If you're going submit a pull request, submit the pull request as early as possible with a WIP in the title. You'll open the door for feedback right from the start and greatly increase the chance of the pull request getting merged.

### What’s your development environment right now?

Atom + Hyper + Chrome

I like to keep things simple because tools and techniques seem to change every few months. Atom and Hyper have packages that minimize the risk of change. Chrome has extensions and probably the best dev/debug tools around.

### What was your first development environment? Do you miss anything from it?

MS Dos + MS Dos Editor (edit command) + C compiler (no idea which one)

I got my first taste of coding around 8 (1995ish?) wrote a simple program to display the result of adding two numbers. After that I didn't touch programming again until learning how to hack the game Counter Strike. I don't really miss anything from the environment, but I think simplicity became a common theme in every iteration of my development environment. I've stayed away from IDEs as a result.

### Where do you see the open source software community headed?

I think that in the next 10 years there will be more people contributing to OSS than the last 10 years. As a result there will be more companies sponsoring OSS projects in the next 10 years. I think as a community we need to hold company sponsored OSS project to a higher standard than those made by volunteers. If we do that I believe we can keep the nice things we have and continue down a sustainable path.
