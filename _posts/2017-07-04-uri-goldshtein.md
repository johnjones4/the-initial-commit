---
layout: post
title: "Uri Goldshtein"
image: "uri.jpg"
seo_title: "An Interview With Angular's Uri Goldshtein"
description: "I was an Angular developer from very early on and really believed in that framework and the team behind it."
links:
  - name: github.com/Urigo
    url: https://github.com/Urigo
projects:
  - name: Angular-meteor
    link: https://angular-meteor.com/
  - name: Angular2-apollo
    link: http://dev.apollodata.com/angular2/
  - name: Meteor-rxjs
    link: https://github.com/Urigo/meteor-rxjs
tags: ["angular", "meteor", "javascript"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

[graphql-subscriptions](https://github.com/apollographql/graphql-subscriptions) - GraphQL Subscriptions is the part of the GraphQL protocol that lets you push real time data to your clients. There are many exciting things about that but for me the most interesting thing is we now have the option to have an open source standard for real time communication, unlike other real time solutions that dictate their own unique proprietary protocol. This library was the first implementation for Node users and helped shape the standard itself and the community around it together with Facebook. The best part in this work that the Apollo team and our community has done was to go on stage together with Lee Byron to announce the official addition of GraphQL Subscriptions to the spec.

[Angular-meteor](https://angular-meteor.com/) - I was an Angular developer from very early on and really believed in that framework and the team behind it.  I also very very impressed my Meteor and it’s philosophy and goal - to create an open source Javascript platform.  So I had two reasons - one was to let me use both in order in my own projects, and second - to share knowledge between the two communities.  Also I’ve created [this manifesto](https://angular-meteor.com/manifesto).

[apollo-angular](https://github.com/apollographql/apollo-angular) - Meteor has been around for 5 years and we constantly thinking about where the ecosystem is heading next and how to progress the platform.  One major thing that happened is that Facebook open sourced GraphQL. At Meteor we saw the GraphQL solves a lot of the same problems we solved with the DDP protocol but also solves many more problems and is in general better for most use cases and more widely adopted by the community.  So we look at it as kind of like DDP 2.0.  Because we want to give our community a chance to upgrade to it gradually, we created separate libraries that anyone can use in their existing apps. My goal here was very similar to angular-meteor - expose the Angular community to the benefits of using GraphQL and giving them a solution to make it easier for them.

[Tortilla](https://github.com/Urigo/tortilla) - Framework for creating tutorials.  Tutorials are a huge passion of mine and I feel they never good enough. So I’ve created a framework to help people create high quality, easily updated tutorials. An example result can be shown by this tutorial - https://angular-meteor.com/tutorials/whatsapp2/ionic/setup

[Meteor Client Bundler](https://github.com/Urigo/meteor-client-bundler) - A tool that helps decouple Meteor in order to Leverage the power of Meteor with any client-side framework

[Meteor-rxjs](https://github.com/Urigo/meteor-rxjs) - Here I’ve done the same but the other way around. The Angular community has really gathered around the concepts of reactive programming using rx-js, so I’ve decided to expose an RxJS API over Meteor’s Collections in order to expose the Meteor community to this great idea and give them tools to use it on their existing apps.

In general I think that programming should be much easier than it is right now and that sharing ideas between the communities would really help with that.


### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I think both. I started it by solving my own problem but from the moment I
realized nobody else has done it, I knew I want to share it with the community
and spread it around.

### How has the project evolved since you first got involved or first released it?

We have a huge community of angular-meteor developers. It’s really inspiring to
see. Almost everyday I get an email from someone who has an app built with
angular-meteor.

One of the things I like the most is that people really appreciate the tutorials
I’ve created for it. I always wanted to write a tutorial for a complete app,
start to finish, and now  I see it was helpful for others as well.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I guess a bit of all.  Luckily I’ve found great people in the community that
help me with each one of those so it’s easier. Also a thing that I really like
is to meet with production users, learn from them about their problems and help
them find the right solutions.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The thing I like that most about the community of angular-meteor is that it is
very diverse. I get to talk with people all over the world, in places I didn't
even know about, and all genders. I don’t know how it became like that. Maybe
it’s because the tutorials make it easier to start even if you are a beginner.

Things that I don’t like are when people don’t see the big picture. What I mean
is that everyday a new cool Javascript library is created.  So people get angry
very fast about why aren’t we using this or that. But when you look at the
bigger picture - the platform - you understand that it’s not about moving fast
but about moving in the right direction. You should really think what is that
library really solving and how does it compare to your current solution.

Another thing that is bugging me is that people are afraid to dig deep in the
code. That means that they when they have a problem or want to integrate a
library, they will open an issue but will do very little in order to understand
what’s happening and how to solve it, even if it means changing the code of the
library.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

I feel responsibility for the community.  I gave lectures to a lot of people, telling them they should use this technology and bet on it.  So I want to keep them happy and productive.

That’s why I’m really focusing now on GraphQL.  I really think it’s not only the right solution for the whole programming community, but especially the right solution for the current users of angular-meteor.

Also, I have this weird idea in my head that most people would probably disagree with - open source libraries should be under a person's name and not under Github organization.

I believe that in this way maintainers will have to take more responsibility because it reflects directly to them.  In a company, small things might get lost because the company might go in a different direction. It can also happen with individuals but I feel it will happen less.

Also, it’s easier to move things around if it’s under a person’s name, meaning, easier to fork and move the community around.  With an organization people follow the organization and not the code, the power of the organization is too big.


### What is the most important thing someone submitting an issue or patch should know?

That everyone is the same.  They should try to dig deep and think what would I
need to do in order to solve it myself. That way I think they will create better
issues with more details about the problem that will help me solve it quickly.

### What’s your development environment right now?

I use a MacBook Pro, using Visual Studio Code and Webstorm. Still haven’t
decided what better…

### What was your first development environment? Do you miss anything from it?

I used Windows machine with Sisual Studio 6 while writing C++ and MFC. I loved
that the IDE was very powerful and had almost everything you need gathered in
the right way for you.

### Where do you see the open source software community headed?

I think we would start seeing that approach spreading around to other fields. We
won’t want our government software to be closed source. We won’t want any of our
softwares to be closed source, why can’t I send a PR to Google Docs?

Also, we will take the same approach to data. If someone would create a great
social network, we won’t leave Facebook because all of our friends/posts/data
are there, and Facebook won’t let us use this information outside of their
walled garden.  Same with search engines, even if someone will create a better
search engine, Google will still have advantage because it has all of my search
history. But this is my search history, not Google’s.

I think this is unacceptable. And the same thing goes to my bank data and the
data my government has on me. I believe the community will start offering more
and more solutions for that problem.
