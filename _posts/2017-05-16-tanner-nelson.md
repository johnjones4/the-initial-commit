---
layout: post
title: "Tanner Nelson"
description: "I maintain the Vapor web framework for Swift which consists of dozens of Swift 3, Linux compatible packages for creating web services."
links:
  - name: github.com/tannernelson
    url: https://github.com/tannernelson
  - name: tanner.xyz
    url: http://tanner.xyz/
projects:
  - name: Vapopr
    link: https://vapor.codes
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain the [Vapor web framework](https://vapor.codes) for Swift which consists of dozens of Swift 3, Linux compatible packages for creating web services. These packages comprise things like HTTP parsers, WebSocket servers, database connectors, etc.

![Vapor Website](https://cloud.githubusercontent.com/assets/1342803/21065187/ef1d94ae-be2c-11e6-9f96-8bf5de2d33c3.png)

I am also an initial stakeholder of the [Swift Server APIs](https://swift.org/server-apis/) workgroup whose job is building a consistent set of HTTP, networking, and security components into Swift itself.

The motivation behind creating Vapor was simple: I love Swift. Back in January when I created it, I had just finished a long Swift/C++ project using Metal for iOS called [Falling Sand](https://itunes.apple.com/us/app/falling-sand/id1044306700?mt=8). I was looking for a new project to spend my free time on, and my idea behind Vapor was the perfect fit.

![First Commit](https://cloud.githubusercontent.com/assets/1342803/21065148/ba0a65f8-be2c-11e6-8434-174956808959.png)

As for releasing it open source, the reasoning is two fold. First, GitHub is an amazing service and I like using it. They give you unlimited open source repositories for free and the tools there make collaborating with people easy and dare I say fun. Also, it doesn't hurt that open source projects are the perfect complement to a software engineer's resume. Second (and most importantly) good web frameworks are open source. That's just the way it is. Take a look at the "[hot frameworks](http://hotframeworks.com)" out there and you'll see that virtually all of them are open source.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Vapor was ultimately the result of being in the right place at the right time. Boiling it down, I see three clear reasons why I started the project.

1: I was working at a tech startup in NYC wearing many hats, two of which were full-stack developer and iOS (Swift) engineer. Being able to perform these roles in tandem opened my eyes to the need for more compile time safety and better debugging in web development.

2: Swift had just gone open source in December 2015. And, more importantly, Apple had released beta compilers for Ubuntu. This meant that Swift could now run on a majority of the computers that power the internet.

![Swift Open Source](https://cloud.githubusercontent.com/assets/1342803/21065245/39a66ca8-be2d-11e6-84e7-b69312594b15.jpg)

3: As mentioned previously, I was looking for something to do!

Given these reasons, starting Vapor was natural. I had over 10 years of experience working with web frameworks and a passion for writing Swift. So it began.

### How has the project evolved since you first got involved or first released it?

The project has evolved tremendously since that first commit. Really the only things that have remained are the name and the core ideas behind what Vapor should be.

The most amazing evolution has been the growth in the community. Vapor has risen to be one of the top 20 most popular Swift projects on GitHub and the team of people in our [Slack group](http://vapor.team) is about to welcome its 2,000th member.

![Slack 2k](https://cloud.githubusercontent.com/assets/1342803/21122130/620662b6-c09e-11e6-9d65-26c9a8309394.png)

Vapor has grown from a pet project, to the #1 trending repository on GitHub, to a real set of tools that people are using right now to create web services.

I am forever grateful for the gracious contributons that helped Vapor grow and for all of the new friends I have made along the way.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

As Vapor has evolved, so has the role that I play. Initially I worked on the project after work. Often time accidentally staying up until 1-2am after getting in the zone on a new feature.

After only a couple of weeks, though, things started getting more serious. The article on Hackernews was one of the biggest milestones. It led to over 2,000 stars on the GitHub repository in a matter of hours. I can still clearly remember waking up Sunday morning to my coworker calling me: "Vapor is #1 on Hackernews right now!"

![Hackernews](https://cloud.githubusercontent.com/assets/1342803/21065520/c040dad6-be2e-11e6-9dac-0c8fe7b6665f.png)


Shortly after that day, Vapor received an incredibly generous sponsorship from a Danish app development company, [Nodes](https://www.nodesagency.com). This allowed myself and one of the other top contributors to the project to [quit our jobs](https://medium.com/@qutheory/vapor-just-got-real-41ecae7aa9e8#.dhxyt3svv) and go full time on Vapor.

Since then, my role has moved more into managing and maintaining the community and resources behind Vapor. Gone are the days of zoning out in Xcode for 12 hours straightâ€“something that I miss if I'm being honest.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The community is starting to grow into its own. It's on the fringe of being self sustaining which I think is incredible for a project this young. Going through my daily routine of checking Slack, Stack Overflow, and GitHub for questions I'll more and more often see the answers already there from some random person. It's really an incredible feeling to see people understanding and using something you helped create.

That being said, Vapor still needs engineers working full time on it to manage the immense amount of GitHub contributions and feature requests. My least favorite aspect is that big open source projects do need some sort of monetary backing to support full timers. Maintaining those aspects of the project consumes more time than I would prefer.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

Now and for the foreseeable future, Vapor is my day job. This is true for myself, my fellow core developer [Logan Wright](https://github.com/LoganWright), and for the growing number of full-time [Vapor developers](https://www.nodes.dk/vapor-developer/) (if you're interested in being a Vapor dev, join our #jobs channel in our [Slack](http://vapor.team)).

More and more engineers, companies, and apps are using Vapor as we speak. Current estimations show hundreds of new projects per week moving toward hundreds per day in 2017. It's my duty to make sure that these projects continue to receive long-term support and that Vapor's adoption for enterprise solutions sees growth.

### What is the most important thing someone submitting an issue or patch should know?

The most common problem I see with issues on GitHub is that they contain too little information. A good habit to form is putting yourself in the maintainers' shoes when reporting a problem or requesting a feature.

In theory, this should be easy for anyone who's good with a computer. We've all had that family member come up to us with some question like: "I've been meaning to ask, my iPhone photos don't work. How do I fix them?" They then wait patiently for a response they imagine will be something like: "Oh, of course. Photos not working. Unlock the phone, press volume down, then clap your hands. Everything should work now!".

In reality, we're left wondering where to begin. Maybe they can't find the camera app icon, maybe iCloud is not enabled. Probably iCloud is not enabled. Then after a few wasted minutes making sure all the settings on their phone are correct (and considering crazier things that could be wrong) you figure out the real problem is they wish their pictures were less blurry.

![Blurry photo of my cat](https://cloud.githubusercontent.com/assets/1342803/21065568/00aecdf8-be2f-11e6-92ed-4ea1154f1f6e.png)


It's the same problem on GitHub. And, unfortunately, with the amount of traffic large projects see, it's really not practical to spend time trying to figure out what someone meant.

Submitting detailed issues or feature requests (even adding detail to vague ones) is something anyone who wants to help out in open source can do.

### What's your development environment right now?

I use Xcode primarily and sometimes Sublime Text or VIM if I need to make mass edits or work on a remote server. Also, the [Material Theme](https://github.com/equinusocio/material-theme) for Sublime Text is beautiful if you haven't tried it.

![Sublime Text](https://cloud.githubusercontent.com/assets/1342803/21065598/2de1dfae-be2f-11e6-8454-f05b8db03456.png)


In terms of the hardware, I created a Hackintosh the for the first time ever this year. It was really fun and I'd recommend it for anyone who likes tinkering.

### What was your first development environment? Do you miss anything from it?

I've been using Sublime since I can remember. However, learning VIM bindings has greatly improved the speed at which I can program.

As far as Xcode goes, I think that program gets better and better every year. Nothing to miss.

### Where do you see the open source software community headed?

Probably not a shocker, but I think open source is the future.  However, while I do think there are a huge number of reasons why [open source should be the future](https://www.youtube.com/watch?v=Ag1AKIl_2GM), only one thing matters at the end of the day: can companies make money off of it.

Fortunately, the answer is yes. The exact details may not be obvious or even exist for every tech company, but ultimately the following is true: If you have some paid service or tool and you create (or support) an open source service or tool that drives more traffic toward your paid one, you make money.

This monetization strategy can be seen in many open source projects. Take Laravel for instance. The free, open source framework drives traffic to paid [services](https://forge.laravel.com), [tutorials](https://laracasts.com), and [conferences](http://laracon.us). Everyone wins.

And, as an added bonus, companies that give away open source software get the love and good will of the developers that use it. Even if they are still making money in the end.
