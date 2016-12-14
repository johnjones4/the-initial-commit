---
layout: post
title: "James Reeves"
seo_title: "An Interview Ring's With James Reeves"
description: "I maintain around sixty open source projects, so it would take a while to name them all!"
links:
  - name: booleanknot.com
    url: http://booleanknot.com
  - name: github.com/weavejester
    url: https://github.com/weavejester
projects:
  - name: Ring
    link: https://github.com/ring-clojure/ring
  - name: Compojure
    link: https://github.com/weavejester/compojure
tags: ["clojure"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain around sixty open source projects, so it would take a while to name
them all! Perhaps the most prominent ones are
[Ring](https://github.com/ring-clojure/ring) and
[Compojure](https://github.com/weavejester/compojure). Many of the others are
small, perhaps a few hundred lines of code, and specialised, designed to solve
one particular task. I mostly program in [Clojure](https://www.clojure.org/),
and Clojure is a language that tends to lend itself to these sort of compact,
focused libraries.

I release libraries as open source mainly because there's no real value in
keeping them to myself, and a whole lot of benefit to releasing them to the
community. Aside from allowing other developers to contribute fixes and
features, the projects I write also act as a portfolio of work. All of the
businesses I've contracted for have hired me at least in part due to the open
source projects I've been involved in.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Almost all the projects I've been involved in have been a reaction to a specific
problem. Perhaps the only exception is Ring, which was originally created by
Mark McGranaghan.

At the time I was writing Compojure as a "batteries included" web framework for
Clojure, and Mark emailed me about a web server abstraction layer he was
developing, along similar lines to Ruby's [Rack](https://rack.github.io/) or
Python's [WSGI](https://www.python.org/dev/peps/pep-0333/). Eventually I wound
up collaborating with him, and moved most of the code I had written for
Compojure into Ring.

### How has the project evolved since you first got involved or first released it?

Some of the projects I write deliberately don't evolve. When a project is small
and focused, there's often little need to alter it after it's been finished.
[Environ](https://github.com/weavejester/environ), for example, has changed
little since its first release.

Other projects tend to evolve through a predictable accumulation of features.
[Codox](https://github.com/weavejester/codox) is a tool I've written for
generating documentation for Clojure, and a recent pull request improved support
for customizing the look of the output HTML.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

For young projects my time is mostly spent developing. As the project matures I
find myself spending more time on issues or on reviewing pull requests. I don't
find that I do a lot of community management; most of the projects I work on are
too small or specific to warrant any sort of community.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

My projects don't really have what I'd think of as a community around them, but
the wider Clojure community is fantastic. I don't think I've ever had a negative
experience or interaction.

I suppose my favourite aspect would be the community's willingness to adopt good
ideas from other languages. My least favourite aspect is probably that the
community lacks diversity, like much of the tech industry overall. Initiatives
like ClojureBridge are vital for improving this.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

Sometimes a project is at the point where it doesn't need much more involvement.
I might accept bug fixes, but the code itself is essentially complete.

Other times a project is ongoing, but I'm still making use of it in some way.
For instance, I use Codox to document my own libraries, so maintaining and
improving that particular project directly benefits me.

Sometimes a project is both not complete, and one I no longer have a use for. In
those cases my involvement tends to dwindle. If it's still reasonably popular,
like [Lein-Ring](https://github.com/weavejester/lein-ring), I'll try and hand it
off to a new set of maintainers.

### What is the most important thing someone submitting an issue or patch should know?

For issues, it's useful to include as much information as possible. If it's a
feature, provide a rationale and use-case. If it's a bug, provide a stacktrace
or detailed explanation of how the application or library is going wrong.

For patches or pull requests, it's a good idea to look for a "CONTRIBUTING" file
in the repository, or failing that, take a look at some pull requests that have
already been merged. Try and match the style of commits and patches that have
already been approved and applied. Include tests if the repository has a test
suite.

Sometimes patches are issues fall through the cracks and are forgotten about.
While I'm sure other projects might have different policies, I personally don't
mind people poking me about issues that haven't been touched in a few weeks or
months. Chances are they've been overlooked, rather than purposefully ignored.

### What’s your development environment right now?

I use Emacs on a Macbook Air, with Vi key bindings courtesy of
[Evil Mode](https://bitbucket.org/lyro/evil/wiki/Home). I have a pretty involved
[configuration file](https://github.com/weavejester/dotfiles/blob/master/emacs.d/init.el),
with a few ideas borrowed from [Spacemacs](http://spacemacs.org/).
[FiraCode](https://github.com/tonsky/FiraCode) is my font of choice, and
[Leiningen](http://leiningen.org/) is the build tool I use.

### What was your first development environment? Do you miss anything from it?

QBasic running in MS DOS. I'd like to claim nostalgia, but can't think of
anything I really miss anything from it. People expect more from software now,
but the development environments we have today are far better than they were
twenty odd years ago.

### Where do you see the open source software community headed?

That's a question I haven't thought about before. I think perhaps we'll see more
open source tools developed that make heavy use of immutable data. Immutability
in version control is already commonplace via Git, and becoming more popular in
the DevOps sphere, with technologies like [Docker](https://www.docker.com/).

I think we'll also slowly start to see a focus on more distributed networks,
like [IPFS](https://ipfs.io/), and there's a strong connection between
immutability and distributed services. Immutable data can avoid many of the
problems around managing updates in distributed systems.
