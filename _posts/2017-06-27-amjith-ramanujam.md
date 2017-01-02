---
layout: post
title: "Amjith Ramanujam"
seo_title: "An Interview With PGCLI and MYCLI Creator Amjith Ramanujam"
description: "I'm the creator of two projects pgcli and mycli"
links:
  - name: github.com/amjith
    url: https://github.com/amjith
  - name: blog.amjith.com
    url: http://blog.amjith.com/
projects:
  - name: pgcli
    link: http://pgcli.com
  - name: mycli
    link: http://mycli.net
tags: ["python"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I'm the creator of two projects [pgcli](http://pgcli.com) and [mycli](http://mycli.net).

![screenshot](https://raw.githubusercontent.com/dbcli/pgcli/master/screenshots/pgcli.gif){: .img-responsive }

They are
commandline clients for Postgres and MySQL databases respectively. I'm a big
fan of fancy
[REPLs](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop).
When I first started learning Python I came across
[bpython](https://bpython-interpreter.org/) and I was in love. Both pgcli and
mycli were inspired by bpython. Every time I used a REPL for a language or a
database, I'd yearn for something like bpython.

I was approached by [Jonathan
Slenders](https://twitter.com/jonathan_s) who was developing a new python
[library](https://github.com/jonathanslenders/python-prompt-toolkit) to serve
as a replacement for `curses`. I was delighted to hear about the project and
surprised by how simple it was to create a fancy repl using his library
prompt-toolkit.

That was indeed the perfect storm that made these projects possible.

---- confession time -----

That was about two years ago. When I look back on why I created the project,
I'm reminded of a particularly tough time in my programming career. I was
working on a high-profile team with extremely high-performing teammates. We
were working on some of the cutting edge stuff in computer science. I was
trying hard to keep up with my teammates. But no matter how hard I tried, I
felt like I just couldn't catch up to them. I was getting increasingly
distraught due to my inadequacy. I finally left that team and joined a
different team. That was such a blow to my self-confidence, I was looking for
something to boost my confidence. Something that could prove to myself that I
wasn't a failure. Something that will convince me that I can write software
that others found useful. That's when I got the message from Jonathan Slenders
about
[prompt-toolkit](https://github.com/jonathanslenders/python-prompt-toolkit) and
I decided to seize the opportunity.

### If you created any of those projects, were they meant to solve a specific problem you faced or were they born out of a larger opportunity you saw?

Pgcli was created to scratch my own itch. I was on a project that required interacting with Postgresql. Instead of learning how to use psql
effectively, I decided to create a client that fit my own mental model of how
REPLs are supposed to work. I wanted a commandline client for Postgres that
could do magical things out of the box with zero configuration. So I decided to write that commandline client. Since
I'm creatively-challenged I decided to give it the most mundane name possible -
pgcli.

The origin story of mycli, on the other hand, was driven by community request.
After I launched pgcli, I got a lot of requests to add support for MySql. So I
launched a kickstarter campaign to create a clone of pgcli for MySql. That was
an interesting learning experience in marketing. The campaign was a success and mycli was born.

### How has the project evolved since you first got involved or first released it?

When I first released pgcli I thought I would get a few interested users and if
I was lucky I would get maybe one or two pull requests. I was off by a few
orders of magnitude.

Today pgcli has over 5000 stars on Github. We have merged 325 pull requests
from over 60 different contributors. There is a core team with 7
members. It has blown away any of my wildest expectations in terms of adoption and usage.

I recently handed over the maintainer duties to one of our long time core-devs.
I think it's time for a new leadership with a fresh perspective. Also my 4-year-old
and 8-month-old sons take up all of my free time. I'm still contributing features and bug fixes but I'm not in the driver seat anymore.

### How do you spend your time on those projects? (i.e. Developing, managing the
community, triaging issues, etc.)

Time spent varies depending on the development cycle. When I was the maintainer of pgcli, I
would take care of releases, which involved writing the changelog, cutting a
release, uploading the package, announcing it via our blog and promoting via
twitter etc. When I'm not releasing, I'm either answering questions via github
issues or reviewing pull requests. Occasionally I do get to implement fresh
new features, either from our backlog or ideas that
were brewing for a while. The core team does an excellent job of pitching in
with features and bug fixes, so I'm not alone in those duties.

One other important duty as a maintainer is to watch the incoming pull
requests and send out invites to the contributors to join the core team. Our requirements are simple:

1. Contribute at least two pull requests that are more than typo fixes.
1. Be nice.

We have never had a problem with users being mean or unreasonable. In that sense, I've been incredibly lucky.

### How would you describe the community around projects you participate in? What
are your favorite and least favorite aspects?

The community has been fantastic. I created a set of
[guidelines](http://pgcli.com/about) for myself about how I would behave
towards the community. This helped attract folks with the right attitude. When
I invite someone to join the core team, the only request I have for them is to
be nice to people who file issues or pull requests. When we see a bug report or
a feature request that is curt or demanding, it is common to assume malcontent.
But often times it's merely a lack of command over the English language. I get a
lot of requests from Chinese and Japanese users that are written using the help
of google translate. So we try to reiterate their problem in our own words
before starting to work on the issue. This has saved us a lot of time.

The feedback I get for pgcli and mycli has been overwhelmingly positive.
Whenever I'm feeling unmotivated, I just go to twitter and search for 'pgcli' or
'mycli' and that immediately lifts up my spirits. So I'm quite thankful for the
thousands of strangers who have said very nice things about the project.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

It's all about the money. Just kidding. Running an OpenSource project is like running my own no-risk startup.

You get to be the product manager who decides the roadmap. You talk to your
customers (through bug tracker) about their needs. You answer users' questions
thus acting as the customer support.  Write documentation, play the role of an
architect, and of course be an engineer who implements a feature and
does the QA. You also get to dabble in marketing by trying to promote the usage
of your project via blogs, talks, social sites etc.

So if you're thinking about starting a company or joining a startup, this is a
great way to find out if you enjoy these tasks.

I get to interact with some top-notch folks in the core dev team. Reading through their pull requests is often times eye opening and I get to learn something new every time.

Regarding the long term plan, I can't be in the helm 100% of the time. But I've been encouraging my core team to take on more responsibilities whenever possible. This helped me hand over the maintainer responsibilities for pgcli recently. I'm in the process of transitioning mycli maintainer job as well. This should free up some more of my time to work on new features.

### What is the most important thing someone submitting an issue or patch should know?

It's ok to submit pull requests that break the build. Sometimes you might not know how to fix it or it could be passing in Python 2 but not in Python 3. That is totally fine. Just open the PR and ask for help. There is a good chance
we (core team) might already know how to deal with that problem.

It's also ok to send small PRs. Not all PRs have to implement a feature. Fixing typos or formatting is just as valuable. It takes me literally 2 minutes to review and merge tiny PRs, so keep 'em coming.

When submitting a bug report or an issue, be as verbose as possible. Give me all the context you can. That helps a lot. Links to supporting documents are also most welcome.

Most of all I appreciate that you took the time to file a bug report. It shows that you care about making pgcli/mycli better.

### What’s your development environment right now?

 * Shell: [Fish shell](https://fishshell.com)
 * Editor: [vim](http://www.vim.org/)
 * Python Interpreter: [bpython](https://bpython-interpreter.org/) or [ptpython](https://github.com/jonathanslenders/ptpython)
 * Python Debugger: [pdb++](https://pypi.python.org/pypi/pdbpp/) or [wdb](https://github.com/Kozea/wdb)
 * Dev Env: [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/)
 * OS: Mac OS and Linux (Ubuntu)

### What was your first development environment? Do you miss anything from it?

GWBasic. I learned it in high school. I miss a lot of things from it. The thing
I miss the most is the Graphics mode. Typing `screen 9` would switch me to a
graphics mode where I can draw simple circles, lines, polygons etc. It was just
a lot of fun. I once built our solar system in GWBasic with my friend. It was
awesome. After answering this question, I downloaded a GWBasic emulator and spent an afternoon coding BASIC with my son. It was a fun [experience](http://blog.amjith.com/nostalgic-programming).

This was in 1998 (not in the 70's or 80's), I just didn't have access to
modern software like Windows 95 or 98 at that time. I also didn't own a
computer. As part of our high school curriculum, we would get one hour per week
in the computer lab. So I had to write all the programs in my notebook and type
it in during that lab time. This forced me to think about the programs before
writing them. I miss that. These days when I see a problem, I fire up my editor
and start hacking right away without much forethought.

### Where do you see the open source software community headed?

I'm cautiously optimistic about the future of open source software. I love the
idea of open source and it's fantastic to see so many open source projects. But
I'm also seeing a lot of maintainers getting burnt out. We can't continue to
build our foundation on the ashes of burnt out programmers. Some of this can be
solved by supporting maintainers financially, but that can't be the only
way.

We need a way to get companies and users to contribute back. GPL did a
fantastic job of making sure the rights were preserved and programmers weren't
exploited. But somehow we managed to paint GPL as a bad license and shun
projects that use GPL.

I don't have a great solution here, hence my cautious stance.
