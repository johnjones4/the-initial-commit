---
layout: post
title: "Henrik Feldt"
seo_title: "An Interview With Suave Co-Creator Henrik Feldt"
description: "Most of these projects are tooling to use to build services. Customers mostly pay for services; not dev tools. Thus, I think it's a question of efficiencies."
image: henrik.jpeg
links:
  - name: github.com/haf
    url: https://github.com/haf
projects:
  - name: Suave
    link: https://suave.io
  - name: Logary
    link: https://github.com/logary/logary
  - name: Fakta
    link: https://github.com/logibit/Fakta
  - name: Logibit.Hawk
    link: https://github.com/logibit/Logibit.Hawk
  - name: expecto
    link: https://github.com/haf/expecto
  - name: Http.fs
    link: https://github.com/haf/Http.fs
  - name: semver
    link: https://github.com/haf/semver
tags: [".NET", "F#"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

To new a few:

* https://suave.io
* https://github.com/logary/logary
* https://github.com/logibit/Fakta
* https://github.com/logibit/Logibit.Hawk
* https://github.com/haf/expecto
* https://github.com/haf/Http.fs
* https://github.com/haf/semver

Most of these projects are tooling to use to build services. Customers mostly pay for services; not dev tools. Thus, I think it's a question of efficiencies.

I could keep the code closed sourced and it would be beneficial immediately to the maturity to manages to reach during the project timeline. The next project, and the next one after that would probably experience either exponential usage or exponential drop-off of usage for the code.

For example, a command-pattern executor library in a game would become intertwined with the source code of the game which would make it less decoupled; so in the long run it would experience less usage due to the overhead of reuse.

On the other hand, a library the successfully decouples from its originating code-base can be continuously improved when faced with new requirements. With a good test-suite it would even be possible to completely rewrite the innards because the public API functionality is retained. Such a library would probably experience exponential usage.

Suave, Logary, expecto and Http.fs are examples of such projects. Suave was originally invented by Ademar and a bit in, I came along and started pushing the project (which had little-to-no uptake) along. Logary comes from my own needs of a unified logging and metrics library on the .Net platform. Expecto has come a very long way in just the last couple of weeks, seemingly from transcend some invisible barrier to uptake that was there in Fuchu (which it's forked from).

Extrapolating from the above, it's my belief that while that immediate (project|code-base|relationships) takes a slight hit from open sourcing something, it's an example of Kaldor-Higgs efficiency in action; where the sum of the gains from the open sourcing action vastly out-weighs the initial costs. In the medium-to-long run this also benefits the originating project or relationship in a manner that is net positive.

I can be that change I want in the world – a net positive force in the medium-to-long run.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Let's pick Suave, which I'm co-author of.

Definitely a specific problem. I needed to create micro-services on the .Net platform and needed a nice web server to do so. I also wanted the code to be ideomatic to F#.

The missing piece was a web server that could be spawned anywhere. On Windows there's this horrible thing called HTTPACLs that trips everyone up and requires Administrators to get involved – because that operating system was, until Nano, stuck in a single-fat-server-many-services world. Friction and frustration.

There's a lot of potential from making projects that remove friction for people who are trying to get things done. If those projects can also be made in a high-quality fashion, you get Suave, which now has multiple books written about it and is often included in books introducing or advancing F# skills.

### How has the project evolved since you first got involved or first released it?

Logary is about as old as Suave. They've followed very different trajectories. Suave has been a rocket speeding towards the stars ;). Logary is more of a lumbering machine which hasn't crossed the invisible uptake-barrier yet. Expecto's value proposition is very easy to understand, so it crossed the barrier almost immediately after release.

The barrier is an interesting notion and for me it's loosely related to how often one gets mentioned in social media or on github. It's also related to whether people contribute answers on StackOverflow for my open source or are active with pull requests and issues on github. But how to cross it? The most obvious example is Fuchu vs Expecto – you can go to Fuchu and see my closed issues there – the same issues I fixed in Expect made the project cross the invisible barrier.

The other projects I mentioned in the first question but haven't mentioned yet haven't yet crossed the barrier but are well positioned to do so when my other technological bets come true – the software-defined datacenter (via Kubernetes) being one of them.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend a lot of open-source-time – maybe 80% of it – trying to make all my code functionally total to avoid having to fix issues down the line. This basically means writing code that has 'no known bugs' in order to avoid quick-fixes and hacks piling on top of each other.

I set up the necessary community hang-outs, like gitter, github issues, a wiki or readme if needed, a twitter account and a tutorial and API guide.

Then the remaining 20% I triage PRs, tweet about work being done and helping people spread the word of my software and do what they want with it. F# weekly quite often has mentions of projects I'm involved in, so it seems to be working. :)

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

It's hard to mention open source projects without talking about the language world they live in.

I think the community is really great for F#. My favourite aspect of it is its willingness to engage and help everyone get started and beyond. The least favourite aspect is how scared Microsoft is to work *with* the community – the company is a NIH-syndrome sufferer and definitely at peak Enterprise.

Of course, peak Enterprise brings some upsides (as opposed to NIH); like a huge wallet to invest into technology with and the ability to throw people at the problem. Compared to Oracle with Java, Microsoft invests more into bleeding-edge technology like .Net Core, but the main organisational body doesn't seem to realise the gem they have with F#. Thankfully they've released the F# tech stack as Apache 2.0 and .Net Core and its native compilers promise to make F# a first-class server-side citizen on par with Java, Erlang, Python and OCaml.

It would be false to ascribe too much clout to an organisation though – in the long run, the community is what matters. And community is created by being helpful and friendly and encouraging people. That's why I stay, anyway.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

The usual; momentum, skill-set, interest and future plans for them. They're also good knowledge hunting grounds. I have a company founded on a F# platform; qvitoo.com, and I want that company to succeed too. The tech-stack is part of that (albeit I'm probably an outlier when it comes to involvement in the core tech stack in most companies).

### What is the most important thing someone submitting an issue or patch should know?

To enjoy doing it.

### What’s your development environment right now?

I've already open sourced it:

- https://github.com/haf/osx

However, now it also includes VSCode with Ionide.

### What was your first development environment? Do you miss anything from it?

Microsoft Word -94 to create web sites. Then Dreamweaver from Macromedia/Adobe.

No, I don't miss a thing. Computers are much better now.

### Where do you see the open source software community headed?

First of all, I think it's heading towards a larger and more uniform community where the individual language used for a service matters less and less.

Secondly, it's heading in the same direction that it already is; to become larger and better established. I don't know of a single company that doesn't use open source software for building their products.
