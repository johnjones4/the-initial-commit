---
layout: post
title: "Parker Moore"
seo_title: "An Interview with Jekyll's Parker Moore"
image: parkermoore.jpg
caption: "In the VSCO office in Oakland, by <a href=\"https://vsco.co/jgenden\" target=\"_blank\">Joe Genden</a>"
description: "Back in 2008, Tom Preston-Werner wanted a better way to publish a blog and documentation for GitHub projects."
links:
  - name: github.com/parkr
    url: https://github.com/parkr
  - name: byparker.com
    url: https://byparker.com
projects:
  - name: Jekyll
    link: https://jekyllrb.com/
  - name: Octopress
    link: http://octopress.org/
tags: ["jekyll"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

Back in 2008, Tom Preston-Werner wanted a better way to publish a blog and documentation for GitHub projects. On what was undoubtedly a brisk San Francisco evening in October, he, along with Nick Quaranto who was likewise working at GitHub at the time, created autoblog, which is now called Jekyll. I took on the role of Lead Maintainer in January 2013.

Jekyll was OK to work with, but had some kinks. Brandon Mathis created Octopress in 2009 to help make the process of developing a Jekyll site better. It’s a really great project. I was emailing Tom about getting involved in Jekyll and approached Brandon about getting involved in Octopress as well, as they were both so closely linked.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I did not create either project, so I can’t speak for their creators. I can say that they solve a particular problem very well, and both were problems born out of a larger opportunity to make publishing on the web a simple and pleasant experience for those comfortable with the command line. Releasing GitHub Pages was a very interesting way to bring Jekyll to the masses, as folks could begin to work on their site entirely on the GitHub.com interface and have it rendered and served. It was a really cool way for someone to get a personal page up on the web that they made, could be proud of, and could call their own little corner of the Internet.

### How has the project evolved since you first got involved or first released it?

Both evolved considerably since I got involved. Octopress had an upgrading problem: users ran “git clone” to clone down the mainline imathis/octopress repo, and started making changes to it to make it their own. Unfortunately, this meant upgrades were really painful because the code that made Octopress great was sitting in their git history. The Rakefile was the main workhorse of the project, and upgrading that caused all sorts of git conflicts. We worked on improving the Rakefile, fixing bugs, but the biggest evolution was the creation of the Octopress 3 project. It moved everything out into a RubyGem which worked similarly to the Jekyll gem.

Jekyll was distributed as an isolated gem with site sources separate, so it didn’t have the same problem. The problems it faced were more community-oriented. I wanted to build an ecosystem of plugins which were likewise distributed as gems, and I wanted Jekyll to become better at what it did. I took over with Matt Rogers when Jekyll was v0.12.1. We shipped 1.0, which was a huge change in the user experience (especially around the CLI). In 1.3.0, we shipped support for RubyGem-based plugins, which has grown a really great developer community around extending Jekyll. Jekyll has also improved its data model over time, adding arbitrary collections of documents (like posts, but not date-centric), and data files.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

Since I started at GitHub, I have spent most of my time on Jekyll improving the stability and managing the community. It’s quite a large community, perhaps the largest of any single static site generator, and I am still learning how I can organize a team of people to keep the ship running. I still develop a feature here and there, but much less frequently. Reviewing pull requests is also a large amount of my time. I’m sad to say I haven’t worked much on Octopress recently.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Open source is how I really learned to program. I could watch other folks who were much smarter and more talented than me solve a problem. The discussion and the code were all there and were preserved in perpetuity. Open source is a really wonderful way to learn and get involved helping others and contributing to the projects you love, and we definitely have that in the Jekyll community. The shared passion for the project is really empowering.

My least favorite aspect of all leading I have done, both for the Jekyll community and elsewhere, is dealing with burnout and the consequent anger, frustration, and exasperation that often goes expressed in knee-jerk comments. We added a Code of Conduct a while back which makes what folks can’t say and do a lot more explicit, but there’s still the sniping at people’s intellect and motivations that you get with any developer community. You see it in the Linux kernel mailing lists, especially. We’re all very good at dealing with code, but somehow dealing with people well still eludes a great many of us, including me sometimes.

The Jekyll community overall is still strong and vibrant. I have loved watching how our forums took off with hundreds of users in the first month or two. The community on there is really nice and helpful. You have some great theme creators like @mmistakes and some big-time Jekyll contributors like @pathawks helping folks out. And our moderators are excellent. And believe it or not, our IRC channel is still alive and well and is taken care of by the kind `jaybe` (@jaybe-jekyll on GitHub). I love seeing these corners of the Internet nerd out about making static sites and making the software to make static sites more easily.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

With so many great things we’re working on for GitHub Pages, it has been tough in the last year to spend much time involved with Jekyll. I am still involved and still releasing new versions of Jekyll. My real hope is to be able to grow a group of excellent maintainers who dedicate some time each week to help push features, fix bugs, deal with issues and so forth. My colleague Mike McQuaid has done a great job of ensuring that the Homebrew project is taken care of by a team of 6 or 7 core maintainers who all pitch in. We still haven’t gotten there yet and I think part of that is because I haven’t given others the space to make decisions and feel ownership. I think over the long term I want to organize a team and give them the freedom to make decisions and push Jekyll forward. That will necessarily mean that I spend less time in every issue and more time helping to coordinate.

### What is the most important thing someone submitting an issue or patch should know?

Most open source development happens in contributors’ free time. The maintainers are rarely paid to work on the project, and they therefore need to spend the bulk of their time working somewhere so they can put food on the table and pay rent, etc. The most important thing to remember is to be kind and flexible. Spend a few minutes searching Google and GitHub for your issue. Has it already been solved? Very often it has a solution. If you have a show-stopping bug, be weary of the time the maintainers have and do your best to run a patched version of the software until it is fixed and by all means fix the bug if you can. The Ruby community has this great saying, abbreviated MINASWAN, “Matz is nice and so we are nice,” and I think it has gone a long way toward making open source Ruby projects a nice place to be.

### What’s your development environment right now?

Macbook Pro, running Mac OS X. I use vim and TextMate 2 to edit code. I do nearly all my communication on GitHub issues for work, and essentially everything I have is versioned in Git and pushed to a repo on GitHub. For energy, I brew the espresso blend from Bicycle Coffee Company, a local roaster here in Oakland, CA. When everything is just too much, I use my ASICS 33-FA running shoes and the lake nearby to clear my head.

### What was your first development environment? Do you miss anything from it?

My first development environment was an Apple IIe, running Apple BASIC. I miss the 5 1/4” floppy disks that held every program I ever wrote and could be loaded into any machine and run. I miss having every program I ever wrote fit on a floppy disk, and I miss the green on black CRT monitors...

### Where do you see the open source software community headed?

This is such an interesting question, and one that has many sides. On the one hand, I see consolidation around well-funded and well-staffed projects, such as Kubernetes and Go from Google. They are moving quickly and a staff of excellent developers are paid to work on it essentially full-time. There is a premium put on stability in addition to speed of release of new features, and it’s fascinating to see how various projects deal with these pressures.

On the other hand, I see a growing influx of folks just learning how to code who are learning through open source. GitHub has made access to communities a little more inviting. I graduated high school in 2010 and think this started a few years before. Programs like Outreachy and Google Summer of Code are providing opportunities for students to dive into code by way of the open source community. That is a really neat transition to watch and in which to participate. Imagine: a whole generation of developers who learned to program almost entirely through open source. As someone who owes so much of his career to open source, this prospect really excites me.
