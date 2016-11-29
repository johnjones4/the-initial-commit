---
layout: post
title:  "Julian Gruber"
description: "The main projects I’m currently involved in are github.com/level and github.com/datproject."
links:
  - name: github.com/juliangruber
    url: https://github.com/juliangruber
  - name: juliangruber.com
    url: http://juliangruber.com/
projects:
  - name: Level
    link: http://leveldb.org/
  - name: Dat Project
    link: https://dat-data.com/
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

The main projects I’m currently involved in are github.com/level and github.com/datproject.

[Level](http://leveldb.org/) is an organisation of independent developers maintaining Node.js bindings to LevelDB - the key-value store by Google which is used in Google Chrome - and curating the ecosystem surrounding it. Really it is about a lot more than just being able to use LevelDB from Node.js. It’s about creating modular databases, something which has never been done before. Open source is perfect for this as we gain a lot from everyone being able to get involved - from all over the world - and on the other side don’t have any private information to hide.

The [dat project](https://dat-data.com/) is a grant-funder non-profit organisation creating tools for governments, scientists and journalists to share and collaborate on data sets huge and small - in a secure, efficient and distributed way. Also primarily built on Node.js, we create desktop applications, websites, command line tools and just general purpose libraries all surrounding our problem space of distributed work on various forms of data. You can’t really create anything that values privacy and integrity of data without making the source freely available - how else would one be able to verify it’s not doing anything malicious? Plus we get a lot of awesome contributions from developers across the globe, like for example [Paul Frazee](https://github.com/pfrazee) and [Yoshua Wuyts](https://github.com/yoshuawuyts/).

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I was one of the creators of the level project, dat I joined later on. I first got interested in modular databases because I wanted to learn how to write my own databases. Using LevelDB as a building block is perfect for this as it already solves the really hard part, which is the efficient storage and retrieval of data on and from disk. There are many other parts to database design though - how you structure your data, how you expose it to the public, how you handle indexes, authentication, etc. etc. So this is the problem space we iterate on!

We quickly realised though that this goes far above creating databases for educational or experimental reasons: There is real world value here, for real world applications. We didn’t create level because we wanted to get ten thousands of GitHub stars, or get famous, which of course also we didn’t. However we _did_ see an opportunity, in shaping a database system that we are interested in using and working for. And that’s all it is basically!

### How has the project evolved since you first got involved or first released it?

First it was just a single repository, node-levelup, maintained by [Rod Vagg](https://github.com/rvagg) and others, like [Raynos](https://github.com/Raynos) for example. I was introduced to the project as my own LevelDB binding, [leveled](https://github.com/juliangruber/node-leveled), was substantially faster than node-levelup, never the less less usable because it had less features. This made us realise we should join our efforts here and merge the two projects into one, and the most practical way was to apply lessons learned writing leveled to node-levelup, so this is where we went.

Next we learned that we want to split the project into two: The JavaScript part and the C++ part. Then you could swap parts as you wish! This is where it became modular for the first time. However we didn’t really realise what this kicked off until way further on.

As development continued and our team and repositories grew, we figured we’d need a new singular home for our endeavours, hence the level organisation was born. Count in amazing developers like [Dominic Tarr](https://github.com/dominictarr), [Paolo Fragomeni](https://github.com/0x00a) and [Lars-Magnus Skog](https://github.com/ralphtheninja), we even gained enough interest from the community to have our own track of talks at one NodeConf EU!

What will happen next? The ecosystem has grown very mature now, there isn’t terribly much to be done any more, at least not in the core parts. I predict more simplifications, performance improvements and awesome user space modules!

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

With level, I spend my time very reactively, as there’s few core issues to progress on. Whenever there is an accepted bug, I work on fixing it. Whenever there is an issue, I help get it answered. I wouldn’t say I do anything special for this community, I respond as I always do, to any human: I try to help solve issues in code and to help people understand why code and maintainers are the way they are. More often than not you get the chance to offer knowledge beyond what’s strictly necessary to understand an issue, and I really enjoy going this extra mile, so I do benefit too a lot when others to it.

Code wise, I value clean code, clear and concise commit messages, and for each pull request it’s the idea to have changes to the test suite and documentation reflect the changes. Although it can sometimes be quite hard and straining to achieve, it’s even the more important to strive for those principles.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Awesome! I can’t think of a community that I actively contribute to that isn’t made up of awesome people doing awesome things. I’d really have to search to find bad aspects. With level for example everything is very natural. If you have time to do something, or are interested in it, you do it. If you don’t, you simply don’t. There’s no obligation whatsoever, it’s simply a collective of developers interested in a shared goal.

With dat it is a little bit different, as we’re getting paid to do this as well, and this is our job. This by no means means that we don’t naturally feel like working on it, however you simply might see responses more timely and better elaborated.

Ok, I do feel like I should mention at least one bad aspect, but sorry, I can’t think of one! If you see something that can be improved, work on it :) I think that’s what we all agree and work on, so it’s a pretty good place to be in if you ask me.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I work on level because I use it in so many other projects. I work on dat because I believe in it, want to work on it, and it pays my bills. I don’t really plan out my long term involvement though, if the projects stay relevant I will continue working on them, and if not, why bother? I mean, of course, if others use a project that needs to be maintained whereas the maintainers lost interest in it already, that’s a bad situation. But, on one side, maintainers come and go as demand rises and falls, and also I’m so heavily invested in especially those two projects that I can’t see me not working on them for a long time.

### What is the most important thing someone submitting an issue or patch should know?

Empathy. Yes, really, empathy. Not code, not the language, empathy. Understand who the maintainers are, where they’re coming from. Understand what they want to achieve, and how they want to achieve it. It’s not even that hard, just read through the commit history and recent pull requests a bit and you’ll get a good feel for the intentions and rules surrounding the project. Try to follow the project’s style as closely as possible - your pull request ideally looks exactly like one a maintainer would create. This helps your pull request get a quick and fair review, as the maintainers can focus on the actual changes and don’t need to discuss styles and conventions with you first.

### What’s your development environment right now?

My development environment is dead simple: An old 13” MacBook Pro running latest OSX, Vim, Hyperterm and Chrome. I’m not an IDE person and prefer to use an editor that I don’t really know how to use. Just forces you to keep it simple.
What was your first development environment? Do you miss anything from it?

### What was your first development environment? Do you miss anything from it?

If I remember correctly, my first development environment was Notepad++ on some Windows version. I tried Visual Studio and Eclipse and more but their slowness and feature richness always turned me off. I don’t care about development environments really. Actually, I prefer one that doesn’t do much...just me and the code. I don’t even know many vim commands! Focus on logic and write modular code, then there’s no real reason to use an IDE.

### Where do you see the open source software community headed?

I see more people getting paid to do open source work. Everything from developers working on corporate open source projects as part of their corporate job to people working on open source full time, being sponsored by various companies, foundations and developers. There’s more and more ways arising to get paid for open source, and that’s great! See for example the recent funding of [vue.js](https://vuejs.org/) on [Patreon](https://www.patreon.com/evanyou): While this is a first, a first will be followed by more if the model is broadly accepted to work - which as far as I can tell it really does!
