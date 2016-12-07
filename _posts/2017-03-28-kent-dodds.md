---
layout: post
title: "Kent C. Dodds"
description: "I have a lot of projects I maintain. Many of them are "finished" and not actively maintained (because no maintenance is needed)"
links:
  - name: github.com/kentcdodds
    url: https://github.com/kentcdodds
  - name: kentcdodds.com
    url: https://kentcdodds.com/
projects:
  - name: cross-env
    link: https://github.com/kentcdodds/cross-env
  - name: angular-formly
    link: https://github.com/formly-js/angular-formly
  - name: validate-commit-msg
    link: https://github.com/kentcdodds/validate-commit-msg
  - name: webpack-validator
    link: https://github.com/js-dxtools/webpack-validator
  - name: webpack-config-utils
    link: https://github.com/kentcdodds/webpack-config-utils
  - name: p-s
    link: https://github.com/kentcdodds/p-s
  - name: match-sorter
    link: https://github.com/kentcdodds/match-sorter
  - name: ng-stats
    link: https://github.com/kentcdodds/ng-stats
  - name: starwars-names
    link: https://github.com/kentcdodds/starwars-names
  - name: npm-kentcdodds
    link: https://github.com/kentcdodds/npm-kentcdodds
  - name: stack-overflow-copy-paste
    link: https://github.com/eggheadio-github/stack-overflow-copy-paste
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I have [a lot of projects I maintain](https://www.npmjs.com/%7Ekentcdodds). Many of them are "finished" and not actively maintained (because no maintenance is needed). Initially I licensed my projects as open source because I had dreams of them helping others (including myself). Now I still do so, but it's no longer a dream--it's a reality. And it feels great.

Some of my more notable projects include:

*   [cross-env](https://github.com/kentcdodds/cross-env)
*   [angular-formly](https://github.com/formly-js/angular-formly)
*   [validate-commit-msg](https://github.com/kentcdodds/validate-commit-msg)
*   [webpack-validator](https://github.com/js-dxtools/webpack-validator)
*   [webpack-config-utils](https://github.com/kentcdodds/webpack-config-utils)
*   [p-s](https://github.com/kentcdodds/p-s)
*   [match-sorter](https://github.com/kentcdodds/match-sorter)
*   [ng-stats](https://github.com/kentcdodds/ng-stats)
*   [starwars-names](https://github.com/kentcdodds/starwars-names)
*   [npm-kentcdodds](https://github.com/kentcdodds/npm-kentcdodds)
*   [stack-overflow-copy-paste](https://github.com/eggheadio-github/stack-overflow-copy-paste)

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Most of the projects I create are out of a specific need that I have. Often I'll simply be extracting code I've written in an application to be an open source, independent module which I can use in other places (for example: [rtl-css-js](https://github.com/kentcdodds/rtl-css-js)) In some cases, I'll even extract code from other open source projects to do this. For example, [validate-commit-msg](https://github.com/kentcdodds/validate-commit-msg) was originally created by the angular team and I extracted it to an individual module which now gets 30k downloads per month. And [match-sorter](https://github.com/kentcdodds/match-sorter) was extracted from my first real open source project [genie](https://github.com/kentcdodds/genie) because I needed the sorting algorithm for something at work.

There are some projects that I inherited. For example, [angular-formly](https://github.com/formly-js/angular-formly) was originally created by a consulting company called [nimbly](https://gonimbly.com/). I started using it at work and contributing heavily so they gave me the project.

I've been on the other end of that for some other projects. For example, [webpack-validator](https://github.com/js-dxtools/webpack-validator) and [eslint-find-rules](https://github.com/sarbbottam/eslint-find-rules) were originally my projects, but other contributors took them way beyond where I could. I would say that this is another of the reasons I open source my code. So I can hand it off to people who can make it more than I would on my own.

There are definitely some projects that I create and don't expect other people to care/contribute. For example [eslint-config-kentcdodds](https://github.com/kentcdodds/eslint-config-kentcdodds) is my custom [ESLint](http://eslint.org/) config which I maintain and use for all my projects. I don't think anyone else is using that and I don't really care. Also [generator-kcd-oss](https://github.com/kentcdodds/generator-kcd-oss) is a [yeoman generator](http://yeoman.io/) so I can spin up new open source projects really quickly.

And I have a lot of open source projects that aren't intended to be used in applications but more to be instructional. Many of my projects on GitHub are workshops or example applications. Also, [stack-overflow-copy-paste](https://github.com/eggheadio-github/stack-overflow-copy-paste) is an actual module you can use (though I don't recommend it) but it's purpose is to be a safe place for people to try out contributing to open source for the first time.

Another source for my open source work is when I'm preparing the educational material and find something that's not very ergonomic or developer friendly. I'll come up with a good solution and open source that, then I'll use that in my instruction. This is where [webpack-validator](https://github.com/js-dxtools/webpack-validator) and [webpack-config-utils](https://github.com/kentcdodds/webpack-config-utils) came from. In other cases it's just a matter of contributing back to another tool to make it better.

### How has the project evolved since you first got involved or first released it?

I start all of my projects at version 1 and strive hard to follow [Semantic Versioning](http://semver.org/). Many of my projects are still on version 1\. So they have only had new features or bug fixes and therefore haven't changed a lot.

However, several of my projects have changed considerably. Most of the time the core idea remains, but the APIs or implementation can change quite a bit. And sometimes this results in churn that's reflected in the major version number. For example [angular-formly](https://github.com/formly-js/angular-formly) is now at `v8.4.0` and is wildly different from where it was when I inherited it. Much of the major changes occurred while preparing a talk about the library. This kind of thing happens fairly often actually.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

It depends on the library, but normally the first while is spent developing the library. Once it's usable (and people start using it), you start spending a lot more time managing the community and triaging issues. I have strategies for doing this effectively. A big part of this strategy is to work on the community really early on and encourage contribution by others even if it takes a little investment. Eventually, the community can run itself (and sometimes, I can hand the project off to someone else as described earlier).

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I love that the community is full of smart people working on their own problems and helping solve each other's problems. We truly are more than the sum of our parts. That moment I start seeing other people respond to issues/stack overflow/chat on my own projects is a wonderful experience!

Having a (beginner) friendly, welcoming, open, and respectful community is really important to me. For my own projects, I have a [Code of Conduct](http://contributor-covenant.org/) which I think contributes in a great way to a friendly and respectful community. I have fortunately never had to enforce the code of conduct in any of my project communities.

I have seen some really sad things in communities I participate in though. Often it's people being really rude and/or entitled. This is definitely something I actively discourage and before I added my code of conduct I experienced this in some of my projects as well. These days, someone behaving like that would be blocked or get a warning depending on the severity.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

Great question. I'm a firm believer that ["You contribute best to something you use regularly."](https://medium.com/@kentcdodds/open-source-stamina-dafd063f9932) So I expect that I'll continue to contribute as I have the need and I'm using the project myself. For example, I no longer contribute to the development of [angular-formly](https://github.com/formly-js/angular-formly) (which is ok, because it's pretty much done).

I do a lot to automate my projects so maintenance is easier. I use [semantic-release](https://github.com/semantic-release/semantic-release) to automatically release a new version when pull requests are merged. So even with projects I no longer use myself or actively maintain, I can continue to merge pull requests and release new versions (even from my phone!) and I do this often. I still care about the project and people using it, but I have limited amount of time, so doing this is pretty awesome (even for projects that I do use a lot).

### What is the most important thing someone submitting an issue or patch should know?

In my projects, I have a fairly comprehensive `CONTRIBUTING.md` file which describes what I expect in issues and pull requests. It's pretty beginner friendly which I think is important. I also have an `ISSUE_TEMPLATE.md` which GitHub will prefill new issues with where I ask for the information I need about the user's environment and versions.

All of that said, I think the most important thing people should recognize is that open source is supported by real humans who have feelings and priorities. So just be nice, please :) Also, this is not _my_ project, it's _our_ project. You have just as much responsibility to find and fix issues as I do.

### What’s your development environment right now?

I use Mac, [Atom](http://kcd.im/atom), Terminal.app, and Chrome. Not too much more to say about that :) The reason I use the regular Mac Terminal rather than HyperTerm is because [it does not support emoji very well right now](https://github.com/zeit/hyper/pull/1006#issuecomment-265227313). 😔

### What was your first development environment? Do you miss anything from it?

I started out doing mostly Java. I used Netbeans and loved it. I was on Windows. Ummm.... Yeah, I don't miss a thing :)

### Where do you see the open source software community headed?

I think it'll continue to grow and be relevant in more places where it's not really used. Many enterprises have a lot of red tape and I expect to see more of that red tape to be cut.
