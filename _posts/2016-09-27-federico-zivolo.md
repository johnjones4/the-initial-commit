---
layout: post
title:  "Federico Zivolo"
description: "Currently the main open source projects I maintain are Bootstrap Material Design (BMD) and Popper.js."
links:
  - name: fezvrasta.github.io
    url: https://fezvrasta.github.io/
  - name: github.com/FezVrasta
    url: https://github.com/FezVrasta
projects:
  - name: Bootstrap Material Design
    link: http://fezvrasta.github.io/bootstrap-material-design/
  - name: Popper.js
    link: https://popper.js.org/
---
### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

Currently the main open source projects I maintain are Bootstrap Material Design
(BMD) and Popper.js.

BMD was created for fun: I was watching Google I/O when they announced
Material Design, and I thought it looked great and I wanted to use it on my own
projects.

At that time, the only available implementation was the one developed by Google,
the Paper elements of Polymer.

It wasn't what I was looking for because it would have forced me to change my
whole tech stack when I just wanted to use their nice "theme." The solution was
obvious: create a Material Design theme for the CSS framework I was using in
those years which was Bootstrap. Initially I released this project with a custom
license. The idea behind it was to provide a free product for personal use and
sell licenses for commercial purposes. The idea worked quite well, but several
people complained about this homemade license because they could not trust such
a license for big projects.

I decided to change the license to MIT once my time available to dedicate to the
project dropped and I wanted to get more help from the community. A quite
interesting read is this issue when a lot of people gave me advices to choose
the right license: [https://github.com/FezVrasta/bootstrap-material-design/issues/410](https://github.com/FezVrasta/bootstrap-material-design/issues/410)

Popper.js has a completely different story behind it: I worked for a San
Francisco startup for few years and the UI of the application we developed was
pretty simple, but it allowed users to customize the visualized data through
several tooltips and popovers (not that I like this pattern that much). The
company had a fork of the Bootstrap tooltips library modified to work in their
framework of choice. Over the years, it evolved to support edge cases,
particular needs and also stuff that had nothing to do with the purpose of the
library, of course 😅.

In practice, every day or so I ended up patching it, adding a feature, removing
one, fixing a bug and so on.

After we looked around to find a pre-made positioning library without success I
decided to dedicate a weekend to work on a tooltip positioning library that
supported all our needs and would be clean, stable and fast.

Popper.js is the result of this weekend of work (plus several others later!),
and I released it as MIT open source because I knew a lot of people needed a
library like that and nothing out there was as good as mine. Also, it gives
value to my portfolio! 😁

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Both my projects have been created to solve specific problems: BMD to provide an
easy way to adopt Google Material Design in Bootstrap projects; Popper.js to
help people position elements in their UI and possibly provide a good "engine"
to create tooltip libraries.

### How has the project evolved since you first got involved or first released it?

The success of BMD was unexpected. I probably hit a moment when Bootstrap was
very popular and in expansion, and Material Design was just launched and got a
lot of media coverage and attention. This rapidly led to people giving stars to
my project on GitHub, ending up in the trending projects several times. Also,
someone posted my project on HackerNews and it reached the first position!

With the support of so many people (and my little experience with big open
source projects) the project grew fast but never reached a good maturity state.

This project helped me to get a good job in a SF startup, this was awesome, but
drastically reduced the time I was able to dedicate to it.

I even considered closing the project and marking it as unmaintained and
deprecated because of the huge number of open issues and my lack of time to
support the project.

Luckily, one of the contributors decided to adopt it and thanks to him the
number of issues reached a good level. He organized the repository to make it
easy to track the problems and improved the release cycle. Meanwhile, he started
the work to support the version 4 of Bootstrap.

Now he doesn't have time anymore to support the project, and I have some
additional free time so I'm keeping it up and running but a new "full-time"
maintainer is still needed I think.

Popper.js, instead, is a relatively new project, it has few months. With the
help of some friends I managed to advertise it on some websites and we reached a
good position on HackerNews. The project has around 3,000 stars but is not
gaining popularity anymore.

One of the reasons, probably, is the specialized nature of this project. I mean,
unlike BMD, this library is useful only to people that need advanced positioning
tools, so it's not a library for everyone.

I have some good ideas to promote the project and reach more people. For
example, I'm trying to make Bootstrap adopt Popper.js as tooltip library for
their 4th version. Also, I'm going to integrate it with the 4th version of
Bootstrap Material Design.

Getting adopted by two big projects should give it the needed visibility to get
adopted by more people and attract contributors to improve its code.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I'm the primary maintainer of both my projects, so I do a bit of everything
every day. I usually spend the initial time developing the project, writing
clean and maintainable code and good documentation. These three points are
essential for a good open source project because nobody will use your library if
it does nothing 😬, nobody will help you to fix bugs if it's not easy to read
and, nobody will adopt your library in their projects if there's not good
documentation to understand how it works and what it can do.

Once this is done, I focus on the promotion of the project: posting on Reddit,
HackerNews, blogs and so on. For example, Popper.js has been mentioned into a
blog post on CSS Tricks, has been featured on HackerNews and several people
talked about it on Twitter and other social media.

This makes the library popular, people use it, report issues, give suggestions
and you start earning some money from the banner on the project site (usually
just few dollars, but it's a great psychological boost!).

Once a little community has been created, I come back to develop new features
and fix issues until a major release is ready. Then the loop starts again.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I had two completely different experiences, the first one with BMD wasn't good,
the second one with Popper.js has been awesome so far:

BMD gained a lot of attention and the community wasn't very helpful. They just
reported bugs without making sure if the issue wasn't already reported, sent
PRs of very low quality and so on. This probably happened because I wasn't
experienced with open source projects and my project grew too fast to let me
grow with it.

Popper.js attracted a lot of skilled people that helped me with new features,
gave me good ideas and reported good issues.

Probably the new issues templates of GitHub helped a lot, because I was able to
provide a "form" that the users were required to fill. If I read an issue with
missing parts or with the template completely ignored, I closed it without
spending much time trying to help the guy who opened it.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I'm maintaining Bootstrap Material Design because a lot of people rely on it and
I have some side-projects that help me buy some sushi the Saturday night. 🍣

Popper.js is something that I really think people need, I'm working hard to make
big projects adopt it and save them a lot of time.

### What is the most important thing someone submitting an issue or patch should know?

When someone wants to submit an issue, please make sure to provide all the
information requested by the maintainer in its CONTRIBUTING.md or in the issues
template. They may look silly because you know the bug you found is real, but
they are needed to help the maintainer! Please always try to reduce your problem
to the minimum amount of code needed to reproduce the problem. We (maintainers)
receive every day a lot of requests and we must be able to reproduce the problem
quickly because our free time to work on our projects isn't unlimited.

When someone wants to contribute to the code, please first make sure to review
the project license and any contributing agreement, it's boring but this stuff
is needed. 😓

Then, make it clear your intent to work on a specific bug or feature reporting
it on the related issue, in this way the maintainer will be able to help you and
you will be sure that nobody else is spending time on the same issue.

When you send the Pull Request, please add all the needed automatic tests to it
to make it easy to verify the validity of your PR and provide a lot of
information to expose what you did!

### What's your development environment right now?

I have an iMac 5k and a Retina MacBook Pro 15", the iMac is the one I use when I
work from home (most of the times) and the MBP is my travel mate when I fly to
San Francisco.

I use Atom as text editor. I was used to Brackets but lately I had a lot of
problems with it and React development. Atom provides the plugins needed to work
with React and it is fast enough. I really like its UI and the available themes.
It's something really important to me, being the software I use most of the time
every day.

Talking about development tools, I really like Rollup, unlike Webpack. With it I
can create awesome transpiled libraries without having to worry about the final
size.

Other life-saver software I use are: Git Tower, to manage Git repositories;
Google Chrome, to... you know; Sketch, to design UIs; MacDown, to write this
article! 🙃; iTerm 2; 1Password, because I can't even remember my birthday;
F.lux and Look Up, to don't get blind; and LICEcap, to record gifs of the
bugs! 🐞

### What was your first development environment? Do you miss anything from it?

I started my developer career on a tower PC assembled by me. It wasn't really
meant for this task - more for gaming probably. I had a crappy monitor and, you
know... Microsoft Windows.

I was literally scared every time I needed to use Adobe Photoshop or any other
"serious" software because the applications kept crashing randomly and my work
was always lost.

Also, npm was having big problems with the path length limit of Windows, making
it impossible to work with some complex projects.

When I was hired by my first startup, the GPU of my computer exploded (or
something like) and I asked my new boss to buy me a MacBook Pro.

I wasn't really excited by it. I never liked Apple, but the situation was:
Windows = crash, Linux = no Adobe, Mac = no crash, yes Adobe. Luckily Apple had
released Yosemite just few months earlier, I think that pre-Yosemite, OS X was
really difficult to use and not pleasant.

At that time, I was using Adobe Brackets as a text editor. I really miss the
project management of it today. 🙁 I don't think I miss anything else from my
previous development environment. Now I have a nice desk, a room I use as office
(wow!) and also a plastic plant from Ikea! What can I ask more?

### Where do you see the open source software community headed?

I think people have said this since the first computer was invented, but I think
OSS is the future. Huge companies like Microsoft, that always considered OSS an
enemy, are now embracing it and releasing important software as open source. NPM
is the largest list of dependencies on the web and most of them are open source!

Developers that count on open source these days can't be wrong. They will make
experiences much faster and will probably make a name in the open source
community, allowing them to get a great job in some awesome company.
