---
layout: post
title:  "Feross Aboukhadijeh"
description: "I work on projects like Standard, WebTorrent, and Study Notes which are entirely open source."
links:
  - name: feross.org
    url: http://feross.org/
  - name: github.com/feross
    url: https://github.com/feross
projects:
  - name: Standard
    link: http://standardjs.com/
  - name: WebTorrent
    link: https://webtorrent.io/
  - name: Study Notes
    link: https://www.apstudynotes.org/
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I work on projects like [Standard](http://standardjs.com/),
[WebTorrent](https://webtorrent.io/), and
[Study Notes](https://www.apstudynotes.org/) which are entirely open source.

Not everything I’ve worked on over my career has been open source, but most of
it has been. I have 100s of open source projects on
[GitHub](https://github.com/feross) and [npm](https://www.npmjs.com/~feross). I
am able to create lots of value in the world when I don’t restrict how people
can use my work. Publishing things under an open source license lets anyone use
my code however they like.

For example, my business Study Notes is doing quite well at making money even
though the code is available on GitHub. Part of my motivation is to prove that
it's possible to make a profit and share your code with the world :)

Sometimes, as in the case of
[WebTorrent Desktop](https://webtorrent.io/desktop/), being non-profit and open
source can actually be
[a competitive advantage](https://torrentfreak.com/webtorrent-250k-downloads-strong-with-zero-revenue-160827/).

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Out of all my projects, Standard is the one that was most clearly designed to
solve a specific need that I had at a very specific point in time.

While working on WebTorrent, I kept getting useful code contributions that had
minor style or functionality issues, e.g. not matching the existing code style,
forgetting to handle errors, or creating paths in a way that doesn't work
cross-platform ("/" vs. "\"). Whenever this happens, a maintainer can do one of
two things: 1) provide feedback and hope that it gets fixed (anecdotally 50% of
the time, it doesn't because the contributor is too busy, or just goes silent)
or 2) accept the code, but immediately make a followup commit to fix the
issues.

I realized that there's actually a third, better way. With a linter, you can
catch code style issues and bugs *before* a code contribution comes in. That was
the motivation for Standard. Catch style errors before they're submitted in PRs
to save precious code review time by eliminating back-and-forth between
maintainer and contributor.

But because the WebTorrent project is split across dozens of GitHub
repositories, and I didn't want to paste in a multi-hundred line linter
configuration in each project, I created a module (`standard`) that all
repositories could depend on. This made Standard require no configuration, which
was unique among linting tools. It was really easy to enforce consistent style
across all my GitHub projects.

When I first started Standard, I was going to call it webtorrent-style, or
feross-style, since it was literally my own stylistic preferences (plus some
non-controversial error catching rules). But I thought it would be amusing to
pick a very opinionated name, so I chose "standard", which was available on npm
at the time.

Since then, hundreds of thousands of people have adopted Standard. Most are just
happy to have a sane default style guide that takes a few seconds to set up.
Some use it as a way to end the constant bickering over code style that takes
place on their teams.

### How has the project evolved since you first got involved or first released it?

Since the beginning, Standard has been adding new rules as ESLint releases them.
The most important rules are designed to catch errors. But we also add rules to
reduce inconsistent code, i.e. if there are two ways to do the same thing, we
prefer to only allow one way. This makes writing code fater -- as you don't have
to consider all the different ways you could do something. And there will only
ever be the one way across the whole codebase. Standard is all about
consistency.

The `standard` command line program has also gotten a lot faster to run. We use
aggressive caching and only run a single linter (ESLint, instead of
ESLint+JSHint+JSCS, like we did at the beginning). We also use ESLint's
excellent `--fix` feature to provide really great automatic fixing of
non-standard code. Just run `standard --fix`.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend the most time triaging issues and considering new rules.

There is a really delicate balance between enforcing new rules that I would like
to see adopted by the community versus being sensitive to how much work it is to
update your code to the new rules. Before I consider any rule change or
addition, I run a very thorough test suite that runs Standard on around 400
community repos to see what the effects of the rule change would be on the
community. Evolving towards stricter rules, especially ones that enforce the use
of new language features from ES2015 and beyond, needs to be done carefully and
respectfully.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

Standard is maintained by a dedicated group of contributors who work tirelessly
to help triage issues, fix bugs, and debate the pros/cons of new rules.

Standard is an [OPEN Open Source](http://openopensource.org/) project, so
whenever someone makes a significant contribution to Standard, they become an
owner of the project, on both GitHub and npm. As of today, there are 16
contributors in addition to myself. Many of them are popular package authors in
the community: flet, jprichardson, dcposch, mafintosh, dcousens, othiym23,
maxogden, watson, jb55, bret, linusu, timoxley, xjamundx, rstacruz, reggi,
yoshuawuyts.

Standard is a true community effort, and I couldn't do it without all the help
I get from these nice folks <3

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I stay involved in Standard because I feel like it's really valuable to the
community.

> "I deal with all the code style arguments so your team doesn't have to."

Instead of 1000s of teams having the same debates over every ESLint rule, we
have them once in the Standard repo and then we can all move on. It's kind of
ironic that I started Standard so I wouldn't have to talk about style anymore,
and now I do that a whole lot more. But since it's for a good cause, I'm willing
to spend my time this way to help out the community that I love.

### What is the most important thing someone submitting an issue or patch should know?

My inbox is overflowing with issues. Most open source maintainers inboxes are
the same way.

Please include as much information as possible, like the version of the package
you're using, the Node.js version, the OS version, as well as detailed steps to
reproduce the issue.

Also, don't forget to be nice! Almost all open source maintainers are unpaid
volunteers. We're doing this because we love it, but dealing with thousands of
issues over the months and years can really take a toll. If you're mean, you're
less likely to get the help you seek, but worst of all, you contribute to
maintainer burnout.
[Burnout](https://en.wikipedia.org/wiki/Occupational_burnout) is a huge and
underreported problem in open source.

### What’s your development environment right now?

I write everything in JavaScript, in Node.js style. I use Node.js on the server,
Browserify in the browser, and Electron for desktop apps. My text editor is
Sublime Text. I use a Macbook 12" since it's ultra portable and can be charged
with a portable USB battery pack, which makes it very convenient during travel.
I don't mind that it's supposedly an underpowered machine. I switched from a
Macbook Pro a few years ago and haven't really missed it.

As Dominic Tarr
[says](https://twitter.com/dominictarr/status/629992939738005504), "If you want
to write fast software, use a slow computer".

### What was your first development environment? Do you miss anything from it?

I used to make sites with PHP. One of the things I miss is the ease of
deployment. Just FTP your code up to the server and your site is live! Nothing
to configure! You can even edit your PHP source files live on the server,
although [there are risks](http://feross.org/cmsploit/) associated with this.

People give PHP a lot of crap, but it actually deserves a lot of credit for the
things is gets right.

### Where do you see the open source software community headed?

I don't claim to be able to foresee where the community is headed. But I do hope
that we address the open source funding problem. As mentioned before, most open
source maintainers are unpaid volunteers, even though our software is frequently
used by Fortune 500 companies, sometimes in very critical contexts
(security, uptime, etc.).

The OpenSSL project was run by a handful of unpaid volunteers, even though it
powers most of the internet's secure communications and commerce. Recently, the
team got funding from a few big companies and now the lead developer gets paid
full-time. But the other volunteers are still working for free.

We need a better model, because the current one doesn't feel sustainable to me.
