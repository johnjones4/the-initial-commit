---
layout: post
title: "Likid Geimfari"
seo_title: "An Interview With Likid Geimfari"
description: "The main projects I’m currently involved in are and expynent."
links:
  - name: github.com/lk-geimfari
    url: https://github.com/lk-geimfari
projects:
  - name: elizabeth
    link: https://github.com/lk-geimfari/elizabeth
  - name: expynent
    link: https://github.com/lk-geimfari/expynent
tags: ["python"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

The main projects I’m currently involved in are [elizabeth](https://github.com/lk-geimfari/elizabeth)
and [expynent](https://github.com/lk-geimfari/expynent).

[elizabeth](https://github.com/lk-geimfari/elizabeth)  is a fast and easy to use Python library for generating dummy data for a variety of purposes. This data can be particularly useful during software development and testing. For example, it could be used to populate a testing database for a web application with user information such as email addresses, usernames, first names, last names, etc. Elizabeth uses a JSON-based datastore and does not require any modules that are not in the Python standard library. There are over eighteen different data providers available, which can produce data related to food, people, computer hardware, transportation, addresses, and more.

[expynent](https://github.com/lk-geimfari/expynent) is a very small library that provides commonly used regular expression patterns, as the patterns for IPv4, username, datetime and etc. I hate to write regex, so I wrote this library. Expynent can be useful in testing. Expynent is an experimental project.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I originally created Elizabeth for better support of languages with more data.

### How has the project evolved since you first got involved or first released it?

In the early the library called `Church`, but some people think that it's offensive. I renamed library  to Elizabeth. The first versions of this library were primitive and they pulls data from text files. Latest version has support of 20 locales and use JSON files as datastore.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)**

I develop new features and fix bugs if they exist. I answer to questions and suggestions about our libraries. In general, as usual.

### How would you describe the community around projects you participate in?

I think they're great guys. People from all over the world interested in the our project and helps in its development, contributing to the Open Source development. It cannot but rejoice. I think (and i hope) that we have small community around Elizabeth that will work on improvements of the library.

### What keeps you involved in those projects?

I think that the interest in Open Source and the desire to make a significant contribution to its development. And I just love the programming.

### Do you have long-term plans for maintaining your involvement?

Yes, i have. I want to add completely correct support of 30 locales, because at this moment we have only 15 locales and sometime with incorrect data. It is difficult to keep track of the correctness of the data, if you know only two languages from 15. We really need the native speakers in the project, to be sure of correctness of data, and I hope that we will be able to attract them in the future.

### What is the most important thing someone submitting an issue or patch should know?

If you gonna send us patch then you need to write test for your code. It's very important. If you want to open an issue, please describe the problem in great detail. Screenshots and logs will be very handy.

### What’s your development environment right now?

My development environment is: An 14” Asus TP500L which running on Ubuntu 16.04 Gnome, Atom and VS Code for Erlang developing and PyCharm for Python, Guake, zsh + oh-my-zsh, Spotify (sometime i listen music until write code) and Chrome. Also sometime i use Vim, but only for editing small config files. Actually I'm not a big fan of Vim.

### What was your first development environment? Do you miss anything from it?

My first development environment is: 14.5” VAIO on Windows 7 and Microsoft Visual Studio. Yeah, is deadly simple. Yes, i do. I miss to the backlit keys.

### Where do you see the open source software community headed?

As we all can see the developer tools are getting better and easier, than ever. Anyone who wants to can start own project which perhaps even will be popular and will be used in large companies.  I’m especially excited for open source communities, such as the the Elixir and big open source production-ready projects as CouchDB, CoreOS, Docker and etc. They are doing an excellent job organizing their projects and the whole ecosystems (Mix and Phoenix for Elixir is great examples) that are surrounding those projects. I hope that our community is waiting more and more talented people who will do great things.
