---
layout: post
title: "Victor Felder"
image: victorfelder.jpg
seo_title: "An Interview With Victor Felder On Open Source Software"
description: "My open source involvement is split between two types of projects: serious projects and pet projects."
links:
  - name: draft.li/blog
    url: https://draft.li/blog/
  - name: github.com/vhf
    url: https://github.com/vhf
projects:
  - name: Zeste De Savoir
    link: https://zestedesavoir.com
  - name: Free Programming Books
    link: https://github.com/vhf/free-programming-books
  - name: Monomorphist
    link: https://mono.morph.ist/
  - name: V8 Bailout Reasons
    link: https://github.com/vhf/v8-bailout-reasons
  - name: Babel
    link: https://babeljs.io/
  - name: Confusable Homoglyphs
    link: https://github.com/vhf/confusable_homoglyphs
tags: ["javascript"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

My open source involvement is split between two types of projects: “serious” projects and “pet” projects. In the serious category, I’m currently spending most of my time maintaining “[Zeste De Savoir](https://zestedesavoir.com)”, a French-speaking online community and web platform. It was founded by a non-profit association aiming at sharing knowledge, in French, on the Internet. We built a Django application with a forum, a publishing platform, a messaging system, etc. Sharing being a core value of this endeavour, the code is GPLv3 and most of the content we publish is Creative Commons.

The most popular open source project I created is certainly [Free Programming Books](https://github.com/vhf/free-programming-books). Seeing a simple github hosted Markdown file take off like this was quite fun. It quickly became the second most popular project on GitHub and is now available in almost 30 languages. Maintaining all these links is a lot of work, I closed over 1,880 pull requests these last three years, which means more than one a day on average. I soon had to schedule the maintenance time I wanted to allocate to this project in order not to be overwhelmed.

The communities around these two projects are really excellent. I’m fortunate to be working alongside awesome contributors.

My “pet” projects are usually smaller things only I use. Sometimes some people get interested or involved, and they might evolve into more serious things. For example, I spent my last weekends building [monomorphist](https://mono.morph.ist/), an online tool abstracting some intricacies of tracing JavaScript code on various node / V8 versions. It’s related to my attempt to [document V8 bailout reasons](https://github.com/vhf/v8-bailout-reasons), resulting from investigations I did while contributing to [Babel](https://babeljs.io/). Some other pet projects are small utility libraries, like a Python lib to detect dangerous uses of [confusable homoglyphs](https://github.com/vhf/confusable_homoglyphs).

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

It’s probably usually both. I don’t think I ever solved a problem I was the only one having. I’m not sure what such a problem could be.

Publishing something under a free or open source license doesn’t cost much, so I usually think of publishing them as an opportunity to help others. If the cost of maintaining something becomes too high, the maintainer can always step out. We’re not signing for life.

### How has the project evolved since you first got involved or first released it?

All these projects are at various stages. For instance, everyone knows Free Programming Books by now, and I intend to keep maintaining it because it seems to be a valuable resource to the 1.5M people viewing it every year. I haven’t really talked about monomorphist to anyone, so no one knows if it’ll be useful to someone or if it’ll stay as a fun experiment.

Zeste De Savoir has been on a constant growth these last two years and seeing how well people respond to our mission and engage with the community I have good hopes it’ll continue to grow and reach a broader audience. We currently average around 200,000 pageviews a month, so we still have a huge margin for progression. Our codebase is sometimes not as clean as I wish it was, but I think we can be proud to be a (reliable and fast) open source platform, a welcoming community and a first experience in open source for so many contributors.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

It really depends on the project. Managing the community is always an important part, but are they really communities or is it more like individuals interacting with the project (and maintainers) without really having to interact with each other? It depends on the project. Anyway, what I mainly do on this side is thanking the contributors, reassuring new contributors about their capabilities, making sure the code of conduct is clear and respected.

As time permits, I mentor contributors (usually on IRC). Helping someone to create their first PR is very rewarding, you can feel their pride of having found an issue they could solve, having dived into a codebase they didn’t know much about, and having fixed their issue. Guidance can be a real help here, at every stage. Conversation helps a lot: Why do you think this bug happens? Where would look at in the code? Can you try to follow the execution flow?

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

We often talk about how hard it is to start contributing to open source, how intimidating it can be, impostor syndrome, bro culture, etc. We talk about some of the good solutions like codes of conduct, mentoring, etc. What we almost never hear about is the language barrier. Getting involved in open source without speaking English is a tough challenge. I didn’t follow this path but it’s something I have been witnessing with this project: our bug tracker being French speaking, it really stimulates French-speaking people with no previous open source experience to take a first step into the open source world. A first step which is very often followed by many more in many other projects, and not only French-speaking ones after that.

Contributing and how to contribute to open source is something you learn, and it’s not always easy to get in. Just like engineering schools usually start with lectures in the local language and student have gradually more and more courses taught in English, I’m pretty sure having welcoming non-English-speaking open source communities can have a huge impact on helping people from all backgrounds start contributing.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

It usually depends on how many people use the project and how hard it would be to hand it over to a new maintainer. It also depends on how much time maintaining the project requires. Maintaining Free Programming Books takes me two hours a week. Being in charge of Zeste De Savoir takes me ten times that. I have been working part-time lately, it allowed me to spend much more time on open source. As of December 1st 2016 I’ll have started an exciting new full-time job, and because of that I’m planning how to best tone down my activity on some open source projects.

I don’t know where to give this answer but I see good and important reasons to contribute to open source, reasons that keep me involved and reasons that should motivate people to contribute. Without talking about the philosophical aspects of sharing work for free. I think contributing to open source makes you a better developer, a better engineer, and a better person. A better developer because it forces you to dive into unfamiliar codebases. A better engineer because it makes you think about how a project is architected and deployed, and understand the pros and cons of different approaches with the chances of seeing live examples of each of these decisions. A better person because it is a mainly collaborative effort.

### What is the most important thing someone submitting an issue or patch should know?

If we make a list of everything they should know, it would be a long list, and ordering it by importance would be impossible. There are so many things to know. Did they read the CONTRIBUTING file? Does their patch pass all tests? Is the coverage still good? Does the patch come with documentation? Did they accept the CLA? Did they read the wiki? Did they look for an existing issue in the closed issues on the bug tracker using 10 alternative keywords? Does the patch comply with an earlier implementation decision taken during a discussion buried in an unrelated issue?

The most important thing someone submitting an issue or patch should know is that it’s ok to screw up a little.

### What’s your development environment right now?
These days I’m mostly using Atom. I still use Sublime everyday though. I’m not a huge fan of either of them, but as long as they don’t get in my way…

I love my zsh config, my gitconfig, my ssh config, etc. Having aliases and custom functions has a good impact on my productivity.

### What was your first development environment? Do you miss anything from it?

It was probably Gnome on Gentoo ten years ago, with Geany as editor. I don’t miss anything from it. My interests have shifted a bit. Spending a lot of time maintaining my work environment was an excellent learning experience. Having now enough Linux skills, I much prefer to have a low maintenance work environment. A shell and a stable platform are all I need.

### Where do you see the open source software community headed?

I wish more companies would publicly acknowledge how much they benefit from open source. Not only open source software, also freely available resources like documentation — language/framework/tools documentation, high level blog posts about architecting a project or deploying things, detailed articles about specific topics, etc.

I sometimes have the feeling that the tech ecosystem, in which the original hacker culture still plays an important role, is really based on sharing code and knowledge, code sometimes being knowledge and knowledge being freedom.

I admire companies putting resources in open source either by maintaining things, by hiring maintainers, or by open sourcing their things. Companies that have technical blogs explaining how they accomplish their mission or how they solved a particular problem they had. Companies encouraging spending time mentoring colleagues one on one or hosting weekly talks where people can share their fun and interesting technical findings, sometimes not being work related stuff.

Sharing knowledge with everybody, sharing code using a free or open source license, publishing with no paywall. All of this is part of the technical scene and it ought to stay that way.

I’d also like to see more diversity in the open source community. There are already a lot of good initiatives working on this and they are doing an excellent and important job. It is much easier for middle class educated white young cis male to spend their time and energy doing open source and privilege makes this category of people naturally feel at ease. It is too easy to be blinded by privilege. It is therefore a responsibility to stand up for diversity and foster a culture of inclusion.
