---
layout: post
title: "Ruslan Talpa"
seo_title: "An Interview With Ruslan Talpa"
description: "At the moment I am involved in PostgREST which is a standalone web server that turns your PostgreSQL database directly into a RESTful API."
links:
  - name: github.com/sobolevn
    url: https://github.com/sobolevn
projects:
  - name: PostgREST
    link: http://postgrest.com/
tags: ["postgres"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

At the moment I am involved in [PostgREST](http://postgrest.com/) which is a standalone web server that turns your PostgreSQL database directly into a RESTful API.
I have also contributed small patches and features to a few other open source projects.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

PostgREST was started by [Joe Nelson](https://begriffs.com/) and I joined the project in Jun of 2015. The reason behind me joining the project was really that the stars aligned, don't know what else to call it :). At the time I had some free time and was thinking of starting something new and at the same time was catching up on interesting technologies. Based on my previous experience I noticed how much time it takes to create an API powerful enough to support a complex frontend so i decided to do something about it. I made a very basic proof of concept and was looking around if something similar existed. Around the same time Facebook announced the plans to release GraphQL specs as open source. Even only from a few slides/examples released at the time, it immediately clicked with me that this interface to an API is exactly what i was looking for. Again, stars being aligned, during that summer i got into Haskell and was impressed so when i ended up on PostgREST github page it was to obvious to ignore. I saw (in PostgREST) a solid base for my idea, I knew the interface (GraphQL) for it was going to be public soon, it was using using Haskell which by that time (1-2 months) i saw convinced it was the one true way :) and i had a few years of experience of building and using exactly the type of APIs that could be built if somehow PostgREST and GraphQL would be put together.  That is when the idea for [Sub0](http://grpahqlapi.com), my new company was born.

### How has the project evolved since you first got involved or first released it?

My direct involvement started with [Issue #218, Support GraphQL query language](https://github.com/begriffs/postgrest/issues/218) on Jun 25, 2015.
If you read through it a bit, you'll see it did not go so well :), there was pushback from other users although Joe, gracious as ever, politely said it was too complicated to implement. Me being a total Haskell noob, did not know what i was getting myself into so i decided to ignore it and push through. The end result was [Skin](https://github.com/ruslantalpa/skin) Sep 2 2015, which after a month of cleaning up, was merged on Oct 4, 2015 [#295](https://github.com/begriffs/postgrest/pull/295) and became the core of what PostgREST is today. As you can imagine i was quite happy (and full of myself :), my first ever contribution to OSS, deep changes to the target project and in an interesting language like Haskell. Having through most of my career as a dev felt the inferiority complex due to not having a formal training and mostly working with languages like PHP and JavaScript (which are a bit looked down upon, especially PHP), i distinctly remember thinking "See, PHP devs are not so bad, we can build stuff too :)", anyway ... Little did i know that this is only the first step and a very long journey lied ahead. A year and a half followed of cleaning up the interface, refactoring, testing performance and fixing bugs (surprisingly few due to Haskell type system), which only recently was more or less finished with [4.0.0](https://github.com/begriffs/postgrest/releases/tag/v0.4.0.0) release.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

Up until recently I was very much involved with development and most of my time was spent pushing the code/features forward. The last few months i am only replying to issues on github and answering questions on Gitter. Most of my time now goes to releasing an MVP for [Sub0](http://grpahqlapi.com)

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I am not sure how exactly to describe a group of people in general. I would say people that pop in often in the chat and heavily use PostgREST are people with quite a lot of experience in architecting systems and have gotten over the phase "let's build everything ourselves in JavaScript". Most of them are 'polyglots' and look for quality/reliability rather then something being in a language they know/use. I would say i like the fact that the level of discussion in issues is high, people always remembering to check RFCs, considering corner cases. My least favorite thing probably refers to the greater Haskell community and it's tendency to work on libraries rather then tools. Don't get me wrong, i am very grateful those libraries exist (ex. Warp, Hasql), i just think Haskell has a bit to lose by not having "finished products".  There is so much knowledge within the community and i basically look at them like gods (maybe people like Michael Snoyman, Edward Kmett, Stephen Diehl are reading this) :) and i just wish they would come down from time to time and lend us mortals a hand (even only with advice) since i am sure their experience would greatly benefit the project. User facing tools/projects like PostgREST are the best advocates for the language since they are "where the action is", meaning the web. Although, as Stephen put it "unfortunately JavaScript still exists", there is a good reason behind JavaScript dominance, it targets everything web, Haskell ecosystem would benefit from concentrating a bit more on the tools for the web.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

Up until i got involved in OSS i had this romantic/naive view of it, how people are altruistically contributing to the good of the humanity and those evil corporations are just profiting from it. That view changed radically in the last year and I've seen my feelings echoed in [some articles](https://www.zdziarski.com/blog/?p=5948). Today i would not use a (big) OSS project in my stack unless i know there is a commercial entity behind it and i understand exactly what are the benefits for that entity. I am not referring here to small libraries and such, I am talking about big codebases. However well intentioned and altruistic a developer is, OSS does not pay the bills so inevitably big projects that do not really have a "finished" state, will eventually be abandoned or code will stagnate and end in the state of "PRs are welcomed" unless there is someone company interested in the project's success. So i am happy to say what, keeps me involved in the project is commercial interest :). Although i have to admit that after a while, you do get attached to the project would like to see it progressing regardless of my original motivation.

### What is the most important thing someone submitting an issue or patch should know?

The most important part is to submit it, the rest can be worked out. The only thing i would probably suggest to the people thinking of submitting features is to first open an issue and see if the addition is a good idea and if it has a chance to be merged.

### What’s your development environment right now?

Nothing fancy, MacBook Air, Sublime/Atom. I always feel like i should invest some time in setting up my editor with plugins and shortcuts but due to the nature of my project i constantly jump between languages and stacks and can't really afford to setting up the editor for everything that i use. Syntax highlight and the command line gets me most of the way.

### What was your first development environment? Do you miss anything from it?

My first computer was a ZX Spectrum clone with BASIC on it. There is nothing to miss about old tech :)

### Where do you see the open source software community headed?

I have not reflected on such big questions and i am in no position really to give opinions on this. What i would probably hope for is some kind of system of support (moral and financial) for people that do this type of work really out of love for the craft (like Joe Nelson).  
