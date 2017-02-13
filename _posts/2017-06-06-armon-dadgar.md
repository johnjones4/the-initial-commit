---
layout: post
title: "Armon Dadgar"
seo_title: "An Interview with HashiCorp's Armon Dadgar"
description: "About four years ago I co-founded HashiCorp with Mitchell Hashimoto."
links:
  - name: github.com/armon
    url: https://github.com/armon
projects:
  - name: Packer
    link: https://www.packer.io/
  - name: Serf
    link: https://www.serf.io/
  - name: Consul
    link: https://www.consul.io/
  - name: Terraform
    link: https://www.terraform.io/
  - name: Vault
    link: https://www.vaultproject.io/
  - name: Nomad
    link: https://www.nomadproject.io/
tags: ["devops"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

About four years ago I co-founded [HashiCorp](https://www.hashicorp.com) with Mitchell Hashimoto.
The company builds [DevOps tools](https://www.hashicorp.com/devops.html) to provision, secure, and run
infrastructure and applications. The core products we build are all open source, and together Mitchell and
I wrote the initial versions of all of them. As part of HashiCorp, we built Packer, Serf, Consul, Terraform,
Vault, and Nomad. Vagrant was written by Mitchell and pre-dates the company but is part of the portfolio now.
Before starting HashiCorp, I also had a few open source projects that I still maintain including
[statsite](https://github.com/statsite/statsite), bloomd, and a few libraries.

The motivation for all of them is the same in some sense. In my previous role as a developer and architect
at a mobile advertising company we faced various scaling and operational issues. This pushed me to rewrite
large parts of our infrastructure in C for stability and performance reasons, which is why I wrote statsite,
bloomd, and hlld among other projects. I open sourced them because I thought they would be helpful to others
and that the community could contribute features and bug fixes back. Today, the Wikimedia foundation uses
statsite, and several large search and advertising companies use bloomd and hlld.

When those companies started using my open source projects it really inspired me. Before that I didn't think
I could have an impact on companies that I didn't work for directly, and it was a sort of revelation to find
that through OSS I could help people I didn't even know. This definitely motivated me to open source more
of my work, and ultimately gave me the confidence to start HashiCorp with a much bigger vision.

Our vision for HashiCorp was to change the way we build and deploy applications, from development
through production. We had a certain set of philosophies we wanted to promote that we've published
as our [Tao of HashiCorp](https://www.hashicorp.com/tao.html), most of which were not mainstream at
the time. What really have us the confidence to even try was our early experiences in open source.
Mitchell was the primary developer behind the very popular Vagrant tool, and I had a few small OSS
projects mentioned before, and together that gave us the confidence to start HashiCorp.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

All of the projects that I created independently or as part of HashiCorp were meant to
solve a specific problem. Some projects were based on existing software, statsite is
protocol compatible with statsd but written in C. The specific problem we faced were
that statsd did not scale well, but the larger opportunity was that almost certainly
other organizations faced the same problem. That wasn't my motivation, but it was certainly
both a specific problem and a larger opportunity.

The HashiCorp tool suite was similarly driven by a specific problem and a larger opportunity.
We felt that we could take a fresh look at the problems in application delivery and build
a new set of tools that would approach the problem in a different way to be more elegant,
scalable, and easier to use.

### How has the project evolved since you first got involved or first released it?

Of my independent projects, statsite is the only one that formed a small community and now
there are several active maintainers and a GitHub organization that continues to work on evolving
it. The other personal projects are maintained and used, but don't have an active community
as they are more niche in the problem they solve.

The projects that we started as part of HashiCorp have evolved substantially, each of them
now has a team dedicated to the product, some have commercial versions, and all of them have
very large communities with hundreds of contributors and tens of thousands of users. As part of
this we get exposed to so many more use cases, so the projects have grown in their scope,
usability, and functionality.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

The time spent on most of the projects includes everything that you mentioned.
Spending time with the community, either over Gitter, mailing lists, GitHub issues, etc is very
important. I spend less time developing these days, and more focus on the product management
and design questions for the projects.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

I feel very fortunate that the community around the projects I'm involved in are all very
healthy and helpful. I've certainly seen very toxic communities, but haven't experienced it
personally. Most of the folks are genuinely interested in the tools because they are end users
and want it to improve. This means they are generally helpful to new members, quick to help test
new releases, and want to give feedback to improve things. My favorite aspect is probably when people
share their use cases and "tips and tricks", as many of these are power tools with no one right way
to use them. My lease favorite aspect is probably the shear volume, as the communities are so large
it takes quite a bit of time just to stay current.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I'm very lucky that my day job keeps me involved with most of the projects. That said, I stay
involved because I really love the products and the problem space. DevOps sits at the intersection
of distributed systems and systems engineering which are two of my favorite topics. Long term,
my plan is to build up the community and hire developers who can be more involved day-to-day so that
I can still remain involved from a product management and architecture perspective.

### What is the most important thing someone submitting an issue or patch should know?

Context is king! The most helpful issues and patches are the ones that explain the _why_
or provide the context. Basic things like what the version number is or the configuration,
though to more complex things like what is the problem you are solving or the use case.
Having context can help reproduce the bugs more quickly, but also helps the core team understand
why a feature ask is being made.

### What’s your development environment right now?

I keep things fairly simple. I develop on my MacBook Air running OSX primarily.
My developer environment is iTerm 2 with Neovim, and using [Vagrant](https://www.vagrantup.com)
when I need to develop on other operating systems or if I have a more complex developer environment
needed for a project.

### What was your first development environment? Do you miss anything from it?

My first developer environment was Visual Studio on Windows, which is where I first
learned to program in BASIC. I'm not sure I actually _miss_ anything from it, it was
a fantastic way to learn programming but I certainly have no desire to write anything
in BASIC at this point. I've been a decade long Vim user at this point, so the mental
rut is fairly deep.

### Where do you see the open source software community headed?

This is an interesting question. Certainly I see the OSS community growing rapidly,
as there is a cultural shift towards openness and sharing. Even in the Enterprise community
where HashiCorp operates we see an increasing comfort with open source. That said, I think
we have a lot to figure out in terms of how to make the communities more inclusive and viable
in the long term. The HashiCorp projects are backed by a commercial company which can
pay developers to build and maintain these projects, but certainly that is a luxury not
all projects have. It would be great to find better ways of supporting the projects we use
and depend on so that we can all continue to benefit from open source.
