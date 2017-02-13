---
layout: post
title: "Fritz Vander Heide"
seo_title: "An Interview With Fritz Vander Heide"
description: "My most recent project is PartyUP, a nightlife application for iOS that allows users to view and submit short videos from nearby party venues (bars, clubs, etc). "
links:
  - name: github.com/etherboy
    url: https://github.com/etherboy
projects:
  - name: PartyUP
    link: http://www.partyuptonight.com
tags: ["ios"]
---


### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

My most recent project is [PartyUP](http://www.partyuptonight.com), a nightlife application for iOS that allows users to view and submit short videos from nearby party venues (bars, clubs, etc).  The videos provide context for choosing the next place to go partying by showing the environment at the venues.  Todd Mercer founded [Sandcastle Application Development](http://www.sandcastleapps.com) to create mobile applications and PartyUP is one of our early products.  I implemented the iOS version of PartyUP and the backend for the application based on Todd's concept for the application and a lot of healthy debate about the details.

We feel that PartyUP has a lot of potential beyond helping millennials find the best local parties to attend.  We don't want to stretch ourselves thin by making variations, so we decided to release the iOS application as open source.  We hope to see interest from the community in helping Sandcastle develop the original PartyUP concept *and* forking the project and using it as a base for addressing other markets.  Take a look at [Sandcastles's projects on GitHub](https://github.com/SandcastleApps).

I have created an open source Tarabish project.  Tarabish is a popular card game in Cape Breton, Nova Scotia.  That one is stale but I plan to return to it as time permits.  Sandcastle has plans for more applications to broaden our portfolio, some of which will be made available as open source.

### If you created any of those projects, were they meant to solve a specific problem you faced or were they born out of a larger opportunity you saw?

PartyUP addresses a problem Todd identified and investigated: indecision caused by a fear of missing out on the best party would often result in people failing to get out and enjoying themselves.  We recognized an opportunity to aid these users while also helping event promoters and venue owners attract the partygoers who investigate their options at the last minute.  PartyUP includes a number of revenue generating mechanisms described in the next answer.

PartyUP has been opened up because there are many similar problems it could address with moderate modification.  For example, we are looking into a variation aimed at coffee shop patrons who would like to see what the atmosphere at local venues is like right now.  I prefer a nice quiet coffee experience myself.  Sandcastle wants to pursue completely new challenges, so letting others build on PartyUP to build those variations benefits us all.

### How has the project evolved since you first got involved or first released it?

The core concept of PartyUP has remained remarkably consistent as it evolved:  allow users to share videos from nearby venues and use those videos to aid in party selection.  In terms of attracting users and generating revenue, PartyUP has evolved a great deal.  We started with a simple advertising and venue promotion mechanism that would be paid for by event promoters and venue owners.  We progressed toward implementation of a loyalty program that would be paid for by venue owners.  Finally, we investigated an achievements system that would encourage a wide range of user behaviors, providing rewards provided by venues and big brands.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend most of my time developing these projects, though documentation comes in a distant but significant second place.  If PartyUP takes off as open source, I imagine I will be writing a lot more documentation and coordinating the community efforts around it.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I have answered questions for fellow users of open source libraries and I write up the occasional bug report for the issues I find.  Bug reports have been very well received by people working on the projects but I do find that some people who ask for help using the libraries can be very unappreciative of the answers they are given.  I understand a user may get frustrated by a library, but that is not an excuse for abusing those trying to help.

A few bad apples in a community, those overly ego-driven, defensive, or simply negative can quickly ruin the project if they aren't dealt with.  I look for projects that have an effective means of dealing with bad apples without devolving into exclusive clubs.  Those are the ones that will survive and are worth investing effort into.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I remain involved in PartyUP because its basic infrastructure can be used as a base for a variety of similar applications.  I plan to play a supporting role over the long term.  I will certainly answer questions and fix issues as time permits.

As for my other projects, I plan to continue development and bring them to the AppStore and GitHub.  I will support them as long as they have an audience.

### What is the most important thing someone submitting an issue or patch should know?

Recognize that regardless of talent or fastidiousness, bugs will happen.  Don't be snarky with those who introduce them or crushed when you do so.  On the other hand, test your work before submitting patches.  You can recognize that bugs will happen, but endeavor to make them infrequent.  

I don't believe in completely egoless programming. I have seen too many instances of sloppy code submissions being made by those who were "egoless", it was used as an excuse for being careless.  I think we need ego to drive us to do great work. We just need it to be resilient enough to accept when we have erred and keep going.

### What’s your development environment right now?

I primarily use Xcode and [SourceTree](https://www.sourcetreeapp.com) (git) on my older MacBook Pro and newer Mac Mini. Today I do most of my development in Swift, I have really enjoyed watching it evolve. I use [Cocoapods](https://cocoapods.org) and [Carthage](https://github.com/Carthage/Carthage) for dependency management, both are great tools that have made it very easy for me to use the many great open source libraries available.  I am incredibly grateful to the creators and maintainers of those libraries, they make many of the projects built on them so much more feasible.    

I use a lot of utilities like [SimPholders](https://simpholders.com), [Homebrew](http://brew.sh), [Inkscape](https://inkscape.org), and [XLIFFTool](https://itunes.apple.com/us/app/xlifftool/id1074282695).

### What was your first development environment? Do you miss anything from it?

I suppose it dates me, but my first development environment was AppleSoft BASIC on my Apple II+.  I don't miss BASIC, but the interactive nature of an interpreter is something I miss from time to time.  Swift playgrounds recreate much of that interactive experience.

I used Metrowerks CodeWarrior for my early Mac development, it was a great tool.  I particularly enjoyed PowerPlant, a object oriented C++ framework that wrapped the Mac toolbox and came with CodeWarrior.  I learned a lot about design patterns from it.  Did anyone else find using the occasional Pascal strings from the Mac toolbox in C++ as disorienting as I did?  Ah, the fun of leaky abstractions

I have also used Visual Studio for most of my career, mostly developing embedded software.  It is a great IDE for C++ and C# development and the implementation of the standard libraries are top notch. I have primarily used Subversion and Git for source control.

### Where do you see the open source software community headed?

I believe the open source community has become less activist and more pragmatic.  This has correlated with businesses becoming more active open source contributors though I am not sure if this is cause or effect.  The use of permissive licenses has facilitated business involvement and I think this involvement in open source will expand.  The healthiest projects seem to be those that money making ventures can use and contribute to with little restriction. As such, I believe the worst thing that could happen to most projects would be the adoption of restrictive licenses like the GPL.

I see a tendency for developer-targeted projects like libraries, source control tools, and issue tracking tools to be much more polished and better supported by the open source community than applications for end users.  I think this trend will continue because the developers contributing to open source projects know that fellow developers are most likely to appreciate the effort.  I am fine with this. Share the libraries and tools for building software as open source but let commercial enterprises that are willing to put in the spit and polish effort make software for end users.
