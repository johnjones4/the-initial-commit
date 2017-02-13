---
layout: post
title: "Maxime Beauchemin"
seo_title: "An Interview With Airbnb's Maxime Beauchemin"
description: "My two main projects are Apache Airflow: a "big data" batch processing orchestrator, and Superset (aka Caravel) a data exploration and visualization platform."
links:
  - name: github.com/mistercrunch
    url: https://github.com/mistercrunch
  - name: mistercrunch.blogspot.com
    url: http://mistercrunch.blogspot.com/
projects:
  - name: Apache Airflow
    link: https://github.com/apache/incubator-airflow
  - name: Superset
    link: https://github.com/airbnb/superset
tags: ["python"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

My two main projects are Apache Airflow: a "big data" batch processing
orchestrator, and Superset (aka Caravel) a data exploration and visualization
platform.

Since the early Linux distribution in the late 90's I've always been
interested in open source. I've always wanted to start a meaningful open
source product. Over time that turned into a bucket list item, and eventually
into an overwhelming reality.

Working at Facebook from 2012-2014 I realized just how accessible it was.
Many individual and teams were sharing their code, and we were using open
source software across the board internally.

When I started the conversation with Airbnb in 2014, the people I spoke with
made it clear that
if I was to join Airbnb I could start working on what became Airflow, and that
I could make the project open source if I wanted to. I was super excited
at the opportunity and frankly a bit scared of making the jump, but I knew it
was the right thing to do. Airbnb needed Airflow, the world
needed Airflow, and I knew exactly how to build it!

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

For Airflow, I definitely saw a huge opportunity since the existing projects in
that space were nowhere close to the maturity of the tools I had used at
Facebook and on the proprietary side of
things. It was clear that every
company with a data team needed a solid batch process orchestrator similar
to the one I had been using and contributing to, and I knew there was a
growing need for the product I had in mind.

For Superset, I started the project at 3 day hackathon. The goal was to allow
exploring and visualizing data out of Druid: an up and coming open source
distributed, realtime column store database. At first, I saw a proof of concept
that may help the state
of realtime data at Airbnb, as well as a gift to the Druid community.
After the hackathon and a few weeks
of hobbying around I got a very nice set of features: a very easy-to-use interface, support for
5-6 types of charts,
and a way to make simple dashboards as a collection of charts. It didn't take
long before I
realized I could easily hook this up to work with pretty much
any SQL-speaking database by using the SQLAlchemy Python library. Then I realized
that my product was a competitor to modern "Business Intelligence" tools like Tableau,
Looker, Mode Analytics and Zoomdata to name just a few. This niche is HUGE,
and there's really not a lot of competition on the open source side of things.
Every company needs a way to access and visualize information, and most people
in those companies need to use such a tool every day.

Projecting myself in my cube back at Yahoo! in 2008, I never would have dreamed that it was
possible for me, or anyone for that matter, to build something like Superset!


### How has the project evolved since you first got involved or first released it?

Airflow has a thriving community with close to 80+ companies officially using
it in production, but that's just the tip of the iceberg: those
are the companies who took time to send a PR adding their name to the list!
Absurdly I think that if I was
trying to stop the project with all my might, I could not at this
point as it truly has a life of its own! Pull requests come faster than we can
commit to review them, we have a dozen or so Apache committers from
5-6 companies, meetups seem to organize themselves, and 50-100 people show
up every time we have one.

For Superset, we now have a very solid working product that company can use
in production at scale. The community is growing fast, and has shown
a vivid interest in the product with 10k+ stars on Github, and more issues
and PRs than we can honor. I wish there was a way to know how many people
have installed it, or how many production installations there are. As large as
the popularity is now, it's still very far from fulfilling a small fraction
of its true potential!

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I do a little bit of everything and make sure I spend 2 to 4 hours a day
actually doing what I do best and enjoy most: coding. Over the past year, I've been
taking on a higher level role with the Airflow community, helping setting
the direction of the project internally and externally, though I'm preparing
a mighty comeback soon with sizable contributions this year.

For Superset, I really enjoyed learning React/Redux while building "SQL Lab"
a feature-rich SQL IDE that ships with Superset. I have to admit that my Javascript
level was "enough to get in big trouble" when I started Superset,
and with the help of outstanding frontend engineer Alanna Scott joining the
team I came all the way from the bottom of the deep end to "fairly proficient"
over the past few months.

I spend a good hour or two every day managing the communities, whatever that may
mean that day. I answer questions by improving the docs, meet with users
at some company in the valley, review code, fix bugs, ... I try to limit
the amount of time and energy I throw at it as it's easy to get obsessed
by it all and there's no end to it.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The Airflow community is truly humbling, showing amazing talent and dedication all
around. It's a specialized subset of the Python community which in itself is a truly
amazing bunch of smart, free-minded, no-bs people.

The Superset contributors are great, though this community comes with a higher rate
of confusing questions, occasional entitlement and people that are not quite sure
what a stack trace is while filling a bug report.

One thing that is important to note as you put energy in an open source
community is that the more you put into it, the more it demands from you.
You'd think "if I document this feature, I won't have to explain it anymore,
and I'll be done with it" but in fact as you answer this question 2 related
(or unrelated) questions might pop out faster than the first one came, and so on.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?
I created these projects out of nothingness and
their relevance and potential grows bigger every single day.
There's that tribe feeling which is deeply rooted in human nature,
a solid sense of pride, and some sort of paternal instinct at play.
I'm also fueled by this nice feeling you get when
free, open, collaborative efforts threaten some of the
capitalistic establishment.


### What is the most important thing someone submitting an issue or patch should know?

We're so grateful for any sort of contribution! Truly! But damn we're busy.
There's an employer, coworkers, friends and family that have all sorts of
expectations from us. We'd love to provide the proper mindshare
to your issue and review your code, but it
may just never make it to the top of the todo list.

We enjoy helping the community, but we enjoy even more helping the people who
are participating in the community. If we don't have time for your issue it's
because we desperately need help! So contribute please contribute! Answer a question from the
mailing list, document an obscure feature, write a blog post about the product or
send an easy-to-review bugfix. As you help others,
it becomes easier for the core project team to spend time helping you.

### What’s your development environment right now?

vim

### What was your first development environment? Do you miss anything from it?

OMG no. ASP (pre .NET), Dreamweaver as an HTML editor, IE, VBScript in place
of Javascript. Stuff nightmares are made of.

###Where do you see the open source software community headed?

What's the long term value of something you can duplicate to infinity?
Software wants to be free. Personally I'm planning a career where I exclusively
write open source code. Join the revolution!
