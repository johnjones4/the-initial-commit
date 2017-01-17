---
layout: post
title: "Vladimir Agafonkin"
image: "vladimiragafonkin.png"
seo_title: "An Interview With Leaflet Creator Vladimir Agafonkin"
description: "The project I am most known for is Leaflet, an open source library for interactive maps."
links:
  - name: github.com/mourner
    url: https://github.com/mourner
  - name: agafonkin.com
    url: http://agafonkin.com/en/
projects:
  - name: Leaflet
    link: http://leafletjs.com/
tags: ["javascript","maps"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

The project I am most known for is [Leaflet](http://leafletjs.com/), an open source library for interactive maps. It started 8 years ago out of frustration with existing open source solutions, which were overly complex, bloated, slow and extremely hard to learn for mapping beginners like me. I wanted to create a simple, fast, lightweight alternative.

Eventually it became extremely popular, and is now used by thousands of developers and some of the biggest companies and organizations (Facebook, GitHub, Foursquare, Flickr, European Commission, data.gov, NPR, Washington Post, Evernote among others). See my [Leaflet story talk](https://www.youtube.com/watch?v=NLbyHffKQuU) for how this happened.

In the recent years, I shifted my focus to new challenges and now maintain a few dozen small, focused libraries that solve various computational geometry and geo visualization problems. I [maintain a list](https://github.com/mourner/projects) so as not to forget any one of them. One example is [RBush](https://github.com/mourner/rbush), a state-of-the-art, blazing fast JavaScript 2D spatial index, which is used as a building block for many types of problems in data-viz and geo apps. Many of these modules are a part of a bigger project I work on with the [Mapbox](https://www.mapbox.com/maps/) team — a next-generation [vector maps](https://www.mapbox.com/maps/) ecosystem.

As for motivation, I like to solve hard problems because I love the challenge, and it's extremely rewarding to see your work help others and push the boundaries of what's possible with technology. Especially so with maps, my focus for the last 8 years. Maps are such an important part of daily lives of people in the Internet era, and it's easy to see the impact your work makes. It also has an infinite stream of hard problems to solve.

I'm also privileged to work for an [open source company](https://www.mapbox.com/about/open/), with a culture of sharing and collaboration, where things you work on are open source by default. This is basically a developer heaven, and the last 3 years working for Mapbox were the happiest in my career.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

The only two reasons to create a project for me is either to solve a specific problem, or to learn something new quickly. Often, it will be both. Diving into a project head-first and learning along the way is always the fastest and most efficient way to learn.

When solving a problem, I'm obsessed with simplicity and performance, and will often come up with the fastest and the simplest solution among all similar projects. This approach attracts many developers and contributors, and is very satisfying.

### How has the project evolved since you first got involved or first released it?

Leaflet surpassed all my wildest dreams and attracted a huge, vibrant community around it. There were [440 contributors](https://github.com/Leaflet/Leaflet/graphs/contributors) to the repo from all over the world, and the [plugins page](http://leafletjs.com/plugins.html) now shines with a whopping list of 320+ plugins.

Most importantly, it became sustainable — in addition to hundreds of contributors, there's now a team of 4 core developers that do amazing work moving the project forward, and although I'm also still involved in maintaining it, Leaflet no longer depends on me to strive.

In terms of implementation, it went through several substantial rewrites and big changes, but it stayed true to its original goal — to be simple, lightweight and extensible, and leave the rest to plugin authors. At some point, I even had to _remove_ nonessential features instead of adding more.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I'm lucky to be able to spend my time on those projects as a part of a full-time job (in addition to many late nights not being able to stop working because of too much excitement), so I have enough time for all three. After the initial release, most of the time is probably spent on communication — discussing ideas, replying to issue reports, reviewing pull requests, etc.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Usually the more focused and technical a project is, the easier it is to communicate with people using it — e.g. a quirky computational geometry library often attracts very smart people who give surprisingly deep insights and contributions, and is much less likely to get bug reports in the vein of "This doesn't work I demand fix ASAP!!!" without further details, or "This is terrible for my use case, you suck". Those moments are my least favourite aspect (related read: [Dear JavaScript](https://medium.com/@thejameskyle/dear-javascript-7e14ffcae36c#.3iw990pcl)), although over the years I have learned to take it easier.

The favourite aspect is getting to work with wonderful, smart, talented people all over the world, and seeing your projects used in the wild for truly awesome things.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I stay involved as long as I'm excited, but I also do my best to help users grow into contributors, and don't hesitate to grant push access to others. I wrote about this [in more detail here](https://medium.com/@agafonkin/agree-with-all-the-points-thanks-for-sharing-this-22742cf4fb2).

### What is the most important thing someone submitting an issue or patch should know?

That the person on the other side has very limited resources, and won't do your work for you. If you want your issue resolved or PR merged, do as much as possible to make the maintainer's job responding easier.

For an issue, this means as many details as possible, with clear steps to reproduce, clear description of expected and actual behavior, and a minimal test case.

For a PR, the most important thing is to minimize the amount of changed code, and break down bigger changes into a series of small changes. PRs with a huge diff always take forever to review and merge, if it ever gets to that point. Simpler = better.

### What’s your development environment right now?

Macbook Pro Retina 15'', mid-2012 — this machine aged surprisingly well, considering that I carry it in my bag and use in dusty environments daily for the last 4+ years. No external monitors — I could never get used to those, and it's easier to focus with just one screen. Sublime Text 3 as the editor (tried switching to alternatives, but I just can't live without its amazing speed). Chrome as the default browser and debugging/profiling tool.

I'm working remotely from a [coworking space](https://www.instagram.com/p/BC708wXR7eQ/?taken-by=mournerv) in Kyiv. Working from home is a huge challenge for a father of 2.5 year old twin girls. :)

### What was your first development environment? Do you miss anything from it?

A Windows PC with EditPlus as a text editor and Opera (in its peak days) as a browser. As a development environment, there's nothing to miss at all. I would miss all the games you can play on a PC (especially CRPGs), but it's actually nice to have a separate gaming PC, and keep the laptop for work and communication only.

### Where do you see the open source software community headed?

More and more companies are allowing their employees to work on open source as a part of their job. This is wonderful — I have a feeling that today, more work is done with the intention to advance technology for the benefit of all (as opposed to purely business interests) than ever before in the history of computing. Open source developers are also much less likely to burn out when they can dedicate a part of their work hours to open source. There's much less skepticism from governments and enterprises about using open source software.

Overall, I think the community is now in its best shape ever, and it will only get better.
