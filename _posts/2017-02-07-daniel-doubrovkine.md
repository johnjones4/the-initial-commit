---
layout: post
title: "Daniel Doubrovkine"
seo_title: "An Interview with Artsy's Daniel Doubrovkine"
description: "I mostly get involved in projects by scratching my own itch."
image: "dblock.jpg"
links:
  - name: code.dblock.org
    url: http://code.dblock.org/
  - name: github.com/dblock
    url: https://github.com/dblock
projects:
  - name: Ruby Grape
    link: https://github.com/ruby-grape/grape
  - name: Hashie
    link: https://github.com/intridea/hashie
  - name: Slack Ruby Client
    link: https://github.com/slack-ruby/slack-ruby-client
  - name: MongoDB Ruby Community Projects
    link: https://github.com/mongoid
  - name: Java Native Access
    link: https://github.com/java-native-access/jna
  - name: Waffle
    link: https://github.com/dblock/waffle
  - name: Oshi
    link: https://github.com/oshi/oshi
  - name: Artsy
    link: https://github.com/artsy
tags: ["ruby"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I mostly get involved in projects by scratching my own itch. I'm an active maintainer of [Ruby Grape](https://github.com/ruby-grape/grape) and [Hashie](https://github.com/intridea/hashie), the [Slack Ruby client](https://github.com/slack-ruby/slack-ruby-client) and a bunch of [MongoDB Ruby Community projects](https://github.com/mongoid). I also spent many years doing Windows development and am still somewhat involved in things like [Java Native Access (JNA)](https://github.com/java-native-access/jna), [Waffle](https://github.com/dblock/waffle) or [Oshi](https://github.com/oshi/oshi). There're of course numerous [open-source Artsy projects](https://github.com/artsy) as we are open-source by default.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Most of my open-source work started very small and solved bite-sized problems. I recently picked up Scala as I wanted to learn and contribute to an existing live auctions bidding service. (This is a complex machine that powers [Artsy Auctions](http://artsy.net/auctions), and works with auction houses such as Sotheby's or Phillips.) Going through project issues I noticed a ticket to add code coverage, which seemed like a good place to start. I had to figure out how to enable sbt-scoverage, and then how to publish code coverage artifacts inside Circle-CI. Both being fairly non-trivial I ended up making [two documentation PRs](https://github.com/circleci/circleci-docs/pulls?q=is%3Apr+author%3Adblock+is%3Aclosed).

### How has the project evolved since you first got involved or first released it?

I didn't start my most popular open-source projects, but felt like I could do a good job helping the community. The [Ruby Grape organization](http://ruby-grape.org/) is incredibly active and my job is primarily cheerleading and growing maintainers. People step in and drop out all the time. I get to work with some world-class developers building fairly complex parts, it's very exciting to be helping someone who's a much better programmer than me!

Sometimes, open-source projects forced me to go down a rabbit hole myself. I was contributing to a Node.js [slack-pongbot](https://github.com/andrewvy/slack-pongbot), which was frustratingly difficult. I ended up [rewriting it in Ruby](https://github.com/dblock/slack-gamebot), and extracting a [client](https://github.com/slack-ruby/slack-ruby-client), [bot](https://github.com/slack-ruby/slack-ruby-bot) and [server](https://github.com/slack-ruby/slack-ruby-bot-server) libraries out of it. [Today](http://airmail.calendar/2016-11-20%2012:00:00%20EST) there's an [entire community](https://github.com/slack-ruby) around all these slack projects written in Ruby. 

Other projects are in deep hibernation but are being used by a massive number of people, such as the [Jenkins ANSI color plugin](https://github.com/dblock/jenkins-ansicolor-plugin). I still can't believe I had to write that.

Finally, there're a number of projects that I find embarrassing, starting with [fui](https://github.com/dblock/fui), my most starred personal Github repo that is nothing short of a hack and that I stubbornly refuse to develop further.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I think I spend half my time managing the community and making sure nothing gets dropped on the floor. This means I'll go pickup issues or e-mails that weren't answered. Depending on the project's stage I triage issues (I definitely enjoy assigning labels). My code contributions are often organizational or infrastructural, such as adding [Danger](http://danger.systems/), which replaces a lot of my involvement by a machine. I do occasionally get direct e-mail about potential security vulnerabilities and might code a piece that I find particularly challenging or compelling.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

It's organic and most people participate by "doing". The lack of long term roadmaps or external "business" forces are two of my most favorite aspects. As a member of Artsy's executive team I deal with those every day, and enjoy it, but having no business strategy or development timelines and a lot of empathy and great code is different, refreshing and encouraging. 



Occasionally someone will troll an issue, demand fixes or complain loudly about lack of support. I don't love it, but, thankfully, I was born in ice cold Russia, so I've grown fairly thick skin.   

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

As with all work, I generally tend to want to give away my legos. This means I actively try to create organizations around my open-source projects and work myself out of being involved in them or at least try to reduce risks or bus factor. I stay involved because I feel like I have to or because the projects are interesting. But my long term plan is always to step out before I get hit by a bus and it's too late.

### What is the most important thing someone submitting an issue or patch should know?

The most important thing is to consider the project maintainers' time. The issue should be very specific, well described and immediately actionable. The worst kinds of issues are the "it doesn't work" kind. So before I ever create a ticket I check out the project on my computer and try to write a test that reproduces the problem within the project's environment. If I fail at that, I'll try to do my best to describe the issue like to a 2yo and provide short and concise information. I always ask myself: "If I got this issue, what would I do? Would I be compelled to do something about it? If it's a bug, is there enough here for me to just fix it?". 

Generally, I also recommend reading the contributing guidelines. Some people are very particular and your job is to make the code look like it was written by them.  Don't send me pull requests without periods at the end of your sentences ;)

### What’s your development environment right now?

I'm typing this on my Macbook Pro that runs macOS Sierra on a train to Boston where I'm judging [MIT Hacking Arts 2016](http://hackingarts.com/). My editor is Sublime Text and a am a heavy user of git shortcuts that you can find on Github in my [dotfiles](https://github.com/dblock/dotfiles). I use Chrome. I am not a huge user of tools or gadgets and my entire development environment can be rebuilt from scratch in an hour as long as I have access to my Dropbox and 1Password.

### What was your first development environment? Do you miss anything from it?

My very first development environment was on DOS 5.0\. It wasn't much of an environment and barely had a text editor. Later in the 90s I spent a lot of time in front of a Sun Sparc machine running Solaris and building cross-platform software in C++. I was a big fan of X-emacs. I really miss the sound that keyboard made! I definitely don't miss working with CVS or trying to compile C++ packages with multithreading support on SGI IRIX into which I had to SSH from the other side of the Atlantic through 4 different nodes :)

### Where do you see the open source software community headed?

I'm very excited to see 100% of the world get serious about open-source. Now that even Microsoft is on that bandwagon, there's no question that the entire software world basically runs on open-source software. The next step is to understand that most code is boring and doesn't need to be built again and again. I want to see more companies adopt the "default to open-source" posture where they ask themselves whether a new project has any competitive advantage of being closed instead of wondering how to open-source something later. This solves numerous problems for corporations, including retention and hiring, reduces cost and increases quality of software being written. I think the open-source communities will retain their organic, non-committal nature, while developers get paid by their companies to work towards business goals, in the open. 
