---
layout: post
title: "Chang-Hung Liang"
seo_title: "An Interview With HTTP Prompt's Chang-Hung Liang"
description: "My most popular project is HTTP Prompt."
links:
  - name: github.com/eliangcs
    url: https://github.com/eliangcs
projects:
  - name: HTTP Prompt
    link: http://http-prompt.com
tags: ["python"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

My most popular project is [HTTP Prompt](http://http-prompt.com). The motivation was to save my own time. There was a period of time at my work where I have to fiddle around with HTTP APIs all day long. It becomes time-consuming and tedious pretty soon if you don't have a good tool. So I created HTTP Prompt and released it as an open source software in the hope that others would find it useful. Check out [the story](https://gist.github.com/eliangcs/464a05ab75ac2a44d2e3dc0ac141cbc6) if you'd like to learn more.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

Yes, HTTP Prompt is a just tool that solves one problem - allow people to easily interact with an HTTP server in terminal. I'm not a fan of GUI. I like to do things in terminal, as much as I can. [HTTPie](https://httpie.org) was the HTTP client I used most of the time. The author of HTTPie, [Jakub Roztocil](https://roztocil.co/), did a really good job designing its user interface. But it's still too bare bones for me when comparing to full fledged tools such as [Postman](https://www.getpostman.com/) and [Paw](https://paw.cloud/). HTTP Prompt is designed to enhance HTTPie just like the way people make Vim an IDE with plugins.

### How has the project evolved since you first got involved or first released it?

As of this writing, HTTP Prompt has [eight major releases](https://github.com/eliangcs/http-prompt/releases) and [10 contributors](https://github.com/eliangcs/http-prompt/graphs/contributors). The project is still young. A frequent contributor [@fogine](https://github.com/fogine) and I implemented quite a few features which I think are very valuable to the users. But in overall, the project doesn't change much since I first released it in May, 2016. I'm still the main maintainer in charge of the direction of the project.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I maintain HTTP Prompt in my spare time. I spend most of the time on developing. Recently, I've been trying to promote and build a community by setting up a [project page](http://http-prompt.com) and a [chat channel](https://gitter.im/eliangcs/http-prompt).

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

HTTP Prompt doesn't really have a community - yet. The main reason is that I know little about how people are using HTTP Prompt as we can't track users for such a developer tool. So it's either we have a small number of users or we have many silent users. And I've been trying to grow the community. As mentioned above, I set up a [chat channel](https://gitter.im/eliangcs/http-prompt) to encourage user feedback. I also wrote up [a welcoming contributor guide](http://docs.http-prompt.com/en/latest/contributor-guide.html) to make contribution easier.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I like to build things that I would actually use for myself. Normally I would maintain my involvement until my requirements for that project are accomplished. And if the project happens to be popular, endorsement from the community can really keep my involvement longer.

### What is the most important thing someone submitting an issue or patch should know?

Read the docs and the contributor guide if there's any.

### What’s your development environment right now?

MacOS, iTerm2, Zsh, Neovim and Tmux.

### What was your first development environment? Do you miss anything from it?

I think it was Windows, UltraEdit, and Dreamweaver. I use them to write PHP websites. And no, I don't miss it.

### Where do you see the open source software community headed?

I really don't know. But recently I have read a book titled [Social Archtecture](https://www.gitbook.com/book/hintjens/social-architecture/details) by Pieter Hintjens. The author describes how building a community for a product is more important than building the product itself. And many successful companies already realize that. The best example is Docker, who open sourced their product and build a community all around it. I think there will be more and more companies following this model.
