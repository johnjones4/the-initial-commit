---
layout: post
title: "Andreas Mueller"
description: "By far the biggest project I work on is scikit-learn, for which I am something like co-maintainer."
image: "amueller.jpeg"
links:
  - name: github.com/amueller
    url: https://github.com/amueller
  - name: amueller.github.io
    url: http://amueller.github.io/
projects:
  - name: scikit-learn
    link: http://scikit-learn.org/
  - name: pystruct
    link: https://github.com/amueller/pystruct
  - name: word_cloud
    link: https://github.com/amueller/word_cloud
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

By far the biggest project I work on is scikit-learn, for which I am something
like co-maintainer. I did not start this project and I did not decide on the
license.

I did create the pystruct library for learning structured prediction and the
word_cloud library to create word clouds with python. The pystruct library is
basically my PhD research. I felt frustrated with the fact that for something
that is widely discussed in academia, namely structural SVMs, there is no nice
and easy to use library. So I created my own, and made it available. For
word_cloud, that was more of a toy project. I didn't think it would get any
uptake, but it did. I mostly open sourced it to share what I had done and get
feedback, but also because at that point I made everything I do open source by
default.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

The word_cloud project was something I did to pass the time and learn more about
an (at the time) new feature of cython. So it was more of an exercise for me.
For pystruct, it was created to help me with my PhD research, but with the goal
to become a more general tool.

I don't want to speak for the creators of scikit-learn too much, but they also
had a very specific application, neuroscience, that they wanted to work on.
However, they decided to make the tools more general, so that other fields can
benefit.

### How has the project evolved since you first got involved or first released it?

Scikit-learn was already pretty useful and big when I joined. I was a user
before I was a contributor. However, adoption has massively increased since
then, and scikit-learn is now the defacto standard for machine learning in
Python.

Many of the original contributors are inactive now because they graduated and
don't have as much time any more. That's unfortunate, but we gathered many more
new contributors over the years, and the project is the biggest it has ever
been. While addition of new methods is somewhat slowing down, the sheer amount
of open issues and pull requests is becoming a bit overwhelming.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend most of my time reviewing code and answering questions on the issue
tracker and mailing list. I also try to work on prioritizing issues and steering
the development. I sometimes implement API changes, or contribute quick fixes,
but that's pretty rare these days. I try to keep up with everything that happens
on the issue tracker, but that's around 100 notifications a day.

I'm also in charge of the releases, which means deciding when to release, what
goes into a release, triggering the build bots and publishing the packages. In
practice nearly all decisions in scikit-learn are made unanimously, so there is
not really a lot of deciding going on. My job is more to make sure a release
actually happens, and the project is in decent shape when that happens.

For pystruct, there is little community, and nearly all of the code has been
written by me. There are some users, and by now there are some people other than
me answering questions on the mailing list. But for better or worse, this is
more or less "my" project.

For word_cloud, I mostly reply to questions on the issue tracker and sometimes
I review code. There are few contributions, and many of them I consider outside
of the scope of the project. Sometimes I implement new features, like the
recently added collocation detection, but that's really just for fun.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The community around scikit-learn is really great, and nearly everybody tries to
be helpful. A lot of people are grateful for the work we do, and that shows.
There are some nay-sayers but they are really in the minority.

I really like having API discussions, and finding out how users use the
software. I also love the enthusiasm of many of the contributors. What I don't
like as much is some people reporting usage questions as bugs. That sometimes
happens with scikit-learn, but for word_cloud it's a much larger fraction of the
users.

The most common question is "why can't I import WordCloud" - to which the answer
usually is "you have not installed it in the environment you want to run it in"
or, and this is comes up a surprising amount, you have given the script you are
running the same name as the library (wordcloud) so when you're trying to import
the wordcloud, you are importing the script itself.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I'm not as active on pystruct any more these days, same goes for word_cloud
which I mostly consider "done" from my end. I certainly want to stay involved
with scikit-learn, and that's one of the main divers of my recent career
decisions.

Both NYU and Columbia enable me to keep working on this project. What keeps me
going is seeing how many people use and love scikit-learn, and the value it
brings to beginners and advanced users. Given my familiarity with the project, I
think working on this is one of the highest impact activities I can do.

### What is the most important thing someone submitting an issue or patch should know?

You need to document and test your change.

### What’s your development environment right now?

vim and jupyter

### What was your first development environment? Do you miss anything from it?

I think Borland Delphi. Maybe Visual C++? I don't remember. The auto-complete
and code-hinting was a bit better than in vim, and setting break-points is a bit
of a pain. Though both of these are as much problems with the IDE as they are
with the language.

Dynamic typing makes code completion and hinting much harder, and python and
breakpoints are not friends unfortunately.

### Where do you see the open source software community headed?

I don't believe there is one open source software community. There are many
communities. I'm part of the scipy community, which is quite different from the
core-python community, which is different from the linux community which is
different from the node.js community.

One issue with the scipy community is that there is currently a large body of
research and industry applications relying heavily on this eco-system, but there
is nearly no financial support from either side. It's individuals struggling to
make it work that have to keep the whole ecosystem afloat. I think we need to
put some effort into making this more sustainable.
