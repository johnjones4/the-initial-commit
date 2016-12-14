---
layout: post
title: "James Montemagno"
description: "I maintain around sixty open source projects, so it would take a while to name them all!"
seo_title: "An Interview With Xamarin's James Montemagno"
image: jamesmontemagno.jpg
links:
  - name: motzcod.es
    url: http://motzcod.es/
  - name: github.com/jamesmontemagno
    url: https://github.com/jamesmontemagno
projects:
  - name: Xamarin
    link: https://www.xamarin.com/
tags: ["xamarin"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

This is a pretty loaded question and may look a bit complicated if you look at my GitHub account. While most of my projects are focused on mobile development with Xamarin they touch all areas of the development process, from small libraries, custom controls, full applications, and my Plugins for Xamarin, which is probably what I am most well known for. I believe completely in giving back to the amazing community of Xamarin developers so every app and library I create is open sourced for everyone to look at and use.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

If I focus in on Plugins for Xamarin I was really inspired by the original Xamarin.Mobile open source project that attempt to abstract APIs on iOS, Android, and Windows into a single API for developers. With the rise of Portable Class Libraries and .NET Standard Libraries it was clear to me that developers (including myself) wanted to access all these great native features such as taking photos, connectivity, and battery usage from their shared code, and boom Plugins for Xamarin was born.

### How has the project evolved since you first got involved or first released it?

When I started the Plugins for Xamarin initiative I wanted to drive a huge community around them so more would be developed. I created templates for Visual Studio and NuGet, wrote blogs, and even did YouTube videos on them and overnight they really took of. Personally, I started with a select few that I needed in my personal apps, but soon I found myself wanting more and more plugins. Then I wanted them to add more features, it was so much fun I had a hard time stopping creating more until I had no time. That is when the fun part of Continuous Integration and Deployment for the libraries with Appveyor came in and really saved the projects that were getting more complex.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I would say I maintain around 10 plugins of which 3 are of high maintenance. Some of them get complete re-writes and new features, while others are purely maintenance as they are pretty much feature complete. I spend a lot of time answering GitHub questions from issues and asking for reproductions of bugs or more information. I then go back and try to document these as best as I can of course. I probably spend the most amount of time trying to keep up with new release of iOS, Android, and Windows as they keep changing APIs all the time.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

There is a great community around plugins in general and specifically around my plugins that I created and actively maintain. I highly encourage pull requests for bug fixes or new features and often accept them without not much back and forth. I love when someone becomes just as passionate about the plugin just as I did when I first created it.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I believe Plugins for Xamarin are pivotal for the rapid development of mobile applications across all of these wonderful platforms and I have seen them help so many developers create great apps that I could never see myself stopping. I am planning some sort of convergence of top plugin contributors in some way to really make them feel like an official project, because they are.

### What is the most important thing someone submitting an issue or patch should know?

Oh my…. Hopefully I don’t go off the rails too much here. I think it is really important to file as much information as humanly possible. I have GitHub templates for filing new issues and maybe only 50% of the time they are actually filled out fully. This delays the process if I don’t know the version number, platforms, etc, but to really get things solved providing source code or even a small sample is a huge huge help. If it is a crash I love stack traces as I can read through them really well and diagnose it, but please don’t paste the entire stack trace in the GitHub issue use a Gist! http://gist.github.com and the project maintainer will love you forever.

### What’s your development environment right now?

I would say around 70% of the time I am on my Surface Book (i7 + 16GB ram + 512GB SSD) inside of Visual Studio 2015 for nearly all of my library and app development. I have a lovely Rose Gold Macbook that I do a lot of my iOS development on inside of Xamarin Studio or use as a build machine. It looks really pretty so often I just stare and admire it to pass time.
### What was your first development environment? Do you miss anything from it?

I got really lucky and got to attend my first programming class in high school which was focused on C++ mostly. We actually got to use Visual Studio 6 and it was amazing! We also got to do a lot of programming in Pascal with Turbo Pascal, which may have been my favorite until I found C#.

### Where do you see the open source software community headed?

I think that we will continue to see tools and sites like GitHub evolve to make it easier for developers to not only make their first contribution, but for maintainers to get feedback and manage their projects. It is amazing to watch this community grow and see more and more large companies embrace the movement to open source.
