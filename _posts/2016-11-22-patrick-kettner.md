---
layout: post
title: "Patrick Kettner"
description: "The most popular project I maintain is Modernizr. I actually did not create it, Faruk Ateş did."
image: "patrickkettner.jpg"
hide_image: true
links:
  - name: github.com/patrickkettner
    url: https://github.com/patrickkettner
projects:
  - name: Modernizr
    link: https://modernizr.com/
---

### What project do you maintain and what was your motivation for creating the project and releasing it as open source software?

The most popular project I maintain is Modernizr. I actually did not create it, Faruk Ateş did. I started contributing to the project for a number of reasons. I had used it a number of times, and when I encountered bugs I wanted to fix them more than normal because the project is so widely used. My initial PR to the project was rejected (as it should have been - it was crap) in the kindest and warmest way I could imagine by Faruk himself. I started researching some of their "undetectables" (a list of features considered to not be able to be detected by Modernizr), and found that a couple of them actually were. I started contributing more and more, and eventually took over the project. I love maintaining it because of how challenging it can be to find creative ways to detect new features, and because of how impactful my code ends up being.

### Was the project meant to solve a specific problem, or was it born out of a larger opportunity you saw?

Faruk originally created the project to make feature detection plug and play for the average developer, and reduce reliance on unreliable user agent sniffing.
ion is

### How has the project evolved since you first released it?

Tons! The purpose of Modernizr is the same as it always has been, but we have added literally hundreds of new feature detections. The performance, accuracy, and browser support of them is monitored constantly, and improved as often as possible. The internal structure has changed a multitude of times, the biggest being transitioning from a monolithic kitchen-sink style script, to a completely modular system.

### How do you spend your time on the project? (i.e. Developing, managing the community, triaging issues, etc.)

Lately, it has been nearly 100% on doing another rewrite (this time changing from requirejs to es6 modules). Normally, it is ~50% development, 25% issues, and 25% pull requests.

### How would you describe the community around your project? What are your favorite and least favorite aspects of it?

The community is generally great. It is much quieter than other similar sized projects. I think this is because it isn't something that you really program with like you would with a Babel or a Lodash. You just sort of add it and forget about it. When folks to communicate or contribute, its quite friendly. In my years with the project, there has only been a few instances or anything but happiness and pleasantries. I love how helpful and friendly folks are. The biggest negatives would be the rare occasion when someone is rude, and the guilt that happens when I don't take care of a problem quickly.

### What keeps you involved in the project? Do you have long-term plans for maintaining your involvement?

Knowing how impactful my work can be, and discovering deep dark problems built into web browsers. It is like being a treasure hunt!

### What is the most important thing someone submitting an issue or patch should know?

That they should just do it! SO many people I talk to have comments, or thoughts about the projec,t but don't want to "bother" maintainers. Thats silly. As long as they are respectful, and remember we are humans, working to try to make the internet a little better with our free time, then any and all communication is great. That, and running tests locally is a good idea before sending it in.

### What’s your development environment right now?

My day job is working on a browser (Microsoft Edge). As a result, I have a ton of different dev envs so I can easily test and work in all major browsers. I code in vim (my dot files are here - github.com/patrickkettner/dotfiles), and use Edge and Chrome as my default browsers depending on what OS I am on.

### What was your first development environment? Do you miss anything from it?

An Apple ][e, and no. Literally nothing. I live in the future and pretty much everything is magical

![First Dev Environment](/img/posts/patrickkettner.jpg){: .img-responsive }

### Where do you see the open source software community headed?

Thats a great question, and I am really not sure. Im hoping that there can be more community work around how to deprecate code, and how to hand off projects. Github has normalized and democratized open source for a huge swath of the online world, and I would love to see us welcome newer, younger, and more diverse peoples to all make the world better through code.
