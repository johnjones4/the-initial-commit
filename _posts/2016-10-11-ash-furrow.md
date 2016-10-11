---
layout: post
title:  "Ash Furrow"
description: "I maintain a number of different open source projects, the two biggest categories are Moya and RxSwiftCommunity."
links:
  - name: ashfurrow.com
    url: https://ashfurrow.com/
  - name: github.com/ashfurrow
    url: https://github.com/ashfurrow
projects:
  - Moya
  - RxSwiftCommunity
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain a number of different open source projects, the two biggest
categories are Moya and RxSwiftCommunity. Let’s start with Moya.

Moya is a Swift-first networking library built on top of Alamofire that uses
Swift features like enums and generics to provide compile-time safety around
network calls, as well as first-class support for stubbed network requests in
unit tests. I started while Swift was still in beta, and we have a policy of
inviting anyone to join the organization after their first merged pull request.
Our rationale is available for others to use and we have automated the
invitation process.

RxSwiftCommunity is a collection of community-managed extensions for RxSwift,
the functional reactive programming framework. These libraries extend built-in
iOS components like CoreBluetooth, and Swift data structures like optionals. It
also uses the Moya contributor guidelines.

By biggest motivation to open these libraries and help manage these communities
is to get developers in a mindset where they help each other and see the value
in community-based learning.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

A bit of both, and others have added their own projects to RxSwiftCommunity as
the community has grown. Moya was really born out of an idea of using Swift
features to provide more compile-time safety for things like networking.

### How has the project evolved since you first got involved or first released it?

Moya has evolved the most – approaching eight major releases. People have added
features I hadn’t ever considered, they’ve fixed bugs I never noticed. I don’t
always agree with their approach – sometimes pull requests get closed – but more
often than not I’m convinced that their idea is better.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I try to focus as close to 100% of my time as possible towards community
management: making sure old issues are closed, cutting releases, encouraging
newcomers, that kind of stuff. I spend almost no time coding in Moya, sometimes
I need to help fix our continuous integration (it’s a chore, I’ve got lots of
experience doing it, and it’s important to me).

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

My favourite aspects of the community are how they can self-organize and rally
behind each other to achieve a goal. I wrote no code in the Swift 3 migration
for Moya, it was all community-driven. The toughest parts involve language
barriers: sometimes people say things on GitHub without realizing they can hurt
feelings. My job is to let them know in a way that doesn’t hurt their feelings
either. But it doesn’t happen often, and it’s always been resolved amicably.

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

My long-term plans for Moya are to popularize the style of contributor
guidelines (invitation after your first PR). I am focused on getting as many
projects onto this style of working because I believe it is better. I’ve written
before about how the biggest existential threat to an open source project is
that the maintainers get bored and leave – this happens far too often. By
spreading out the responsibility, the community can shoulder the responsibility
of running the project when the original maintainer leaves.

### What is the most important thing someone submitting an issue or patch should know?

Be polite and kind – you and the maintainer both want what’s best for the
project.

### What’s your development environment right now?

Oh gosh, I’m bouncing between Xcode and VSCode (doing a lot of React lately).
I’ve got a 12” MacBook for home stuff, but I work on a Mac Pro.

### What was your first development environment? Do you miss anything from it?

My first development environment – that could run the iOS simulator, anyway –
was a hackintosh I made from a netbook in 2009. I miss nothing about it.

### Where do you see the open source software community headed?

I see us headed towards a kinder future where companies are far more open with
their technology than they are now. In the future, all software will be open
source by default; that means it’ll be open unless there’s a reason to keep it
secret. This is the opposite of how things are today: secret unless there’s a
reason to open. We’ll get there, through grassroots pushes from developers
inside companies, who will eventually build their own companies with open source
ideals at heart.
