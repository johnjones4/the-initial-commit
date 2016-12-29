---
layout: post
title: "Edward Kmett"
seo_title: "An Interview With Haskell Developer Edward Kmett"
description: "I maintain roughly 125 packages for the Haskell ecosystem on hackage."
links:
  - name: github.com/ekmett
    url: https://github.com/ekmett
  - name: comonad.com
    url: http://comonad.com/
projects:
  - name: lens
    link: http://hackage.haskell.org/package/lens
  - name: linear
    link: http://hackage.haskell.org/package/linear
  - name: OpenGL bindings
    link: http://hackage.haskell.org/package/gl
  - name: hyphenation
    link: http://hackage.haskell.org/package/hyphenation
tags: ["haskell"]
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I maintain roughly 125 packages for the Haskell ecosystem on [hackage](http://hackage.haskell.org/user/EdwardKmett). I have about a hundred more projects sitting on my GitHub account in various stages of completion. The justifications and motivations for each vary widely.

For the most part I look for something that should exist for some deep underlying mathematical reason that doesn't yet exist in code in a reusable form and try to figure out how to bring it about. I gave a fairly general audience talk on "Learning How To Learn" [at YOW! 2014](https://yow.eventer.com/yow-2014-1222/stop-treading-water-learning-to-learn-by-edward-kmett-1750) that dove deeper into how I try to match up problems and solutions.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

My development of a project usually starts out as a form of depth-first development as I try to build a larger project. When I'm nominally working on a larger project I'll drill in and in until I find a sub-problem I can definitively solve, and then ship that once it is as polished as I can make it. Then I pop the stack and go back to work.

Unfortunately my stack is only so deep, so I tend to forget what started me on the path to my current project after a while, which leads me to starting a new grand project, drilling and hoping that some of the holes I'm finding have already been spackled over by previous passes.

An example is the ['lens' package](http://hackage.haskell.org/package/lens), which offers what has become a popular way to deal with mutating state in functional programming. Lenses had existed in the functional programming as a curiosity long before I got involved.

I wrote my first lenses in [Scala](https://www.youtube.com/watch?v=efv0SQNde5Q). At work we have a compiler for a Haskell-like language at my work called [Ermine](https://www.youtube.com/watch?v=o3m2NkusI9k), and in the process of working on the compiler we had to manipulate a lot of deeply nested state inside immutable objects. Lenses let us encapsulate a lot of that code and reduce our boilerplate.

Then I didn't think about lenses much for a couple of years. Eventually I was relaxing by working on a little 2d game engine. I wanted to play around with giving the game AI the ability to run the physics simulation a couple of steps directly, but this meant I needed a physics engine that was actually purely functional -- or which at least had a good snapshot capability.

But if I wanted to do 2d actors that turned into ragdolls when blown up, I really needed sort of mixed 2d/3d physics, otherwise limbs don't bend right and everything looks cheesy. With that I resigned myself to returning to my old game dev roots and writing a little physics engine.

But then I realized there was no good linear algebra library in Haskell to build it upon. So, fine, I've resolved to build enough linear algebra to handle quaternions and rotations and what not for 3-4 dimensional problems. So now I need a good encoding of linear algebra.

My math background is a bit disorganized, but one thing I remembered very well from a book on projective geometry is that all projective geometries are just exercises in [linear algebra](http://www.maths.ed.ac.uk/~aar/papers/beutel.pdf). And another comment I remembered from long nights skimming Wikipedia is that every vector space is a free vector space. (There are modules over rings, such as ideals, that aren't free modules, but not vector spaces over a field.) That is to say every vector space looks like a function from X -> R, where R is a field, and the set X is some set of basis vectors. Basically this is the very boring statement that you can decompose vectors into a sum of scalars times your choice of basis vectors. Unfortunately representing vector spaces as function spaces is rather inefficient, but it is a great conceptual model.

Now, in category theory we have the notion that there are "corepresentable functors" that is to say a functor F, such that F a is isomorphic to X -> a for some object X, which I'll call the representation of that functor. So if I instead decide that all my vector spaces will simply be encoded as these corepresentable functors, most of my problems are solved.

```
data R2 a = R2 a a
```

is isomorphic to a function

```
Bool -> a
```

Now this still requires me to find a choice of basis for each vector space, but it just so happens that lenses can provide a canonical choice of such a basis.

```
(forall x. Lens' (f x) x) -> a
```

And the nice thing is I can use typeclasses to share such lenses between different vector spaces. By giving names to the 'x' dimension or 'y' dimension. I can share those names across 2d and 3d vectors for convenience.

I'd originally planned on using somebody else's library for the lenses, but I found I wanted a bunch of stuff that was just a little too much for the library I was leaning on, so I banged out 20 lines of code and embedded my own directly into the code in question.

At that point I now had a game engine flayed open, a physics engine started, a linear algebra library started, and a 20-line lens library started as the guts of the linear algebra library.

That code grew, a lot, and became a heck of a lot more interesting than the toy game engine of which it was part. So I eventually just took it out and focused on growing a good reusable vocabulary for working with lenses and lens-like structures.

Several months later I showed a robotics researcher some of the code I had had in the linear algebra library for dealing with tricky branch cuts in the quaternion code -- and he insisted that I package it up so that he could use it in his robotics work, so I shipped another package, [linear](http://hackage.haskell.org/package/linear).

Nowadays there seems to be a whole approach to software development in the functional programming community that builds up large states and then drills into them using lenses. This arose mostly among the very pragmatic "get it done and ship it" web development community.

Another package that I've built that has seen surprisingly wide adoption is my 'ad' automatic differentiation library. I wrote it to answer a stack overflow question about reverse mode AD in [Haskell](http://stackoverflow.com/questions/2744973/is-there-any-working-implementation-of-reverse-mode-automatic-differentiation-fo). I tested it with functions of maybe 3 variables. A couple of months later a guy doing computer vision research reached out and said it was a bit slow when using it with 400,000 variables. After fixing that up, somebody contacted me about using it in finance with a 10s of millions of variables. Needless to say all of the eyeballs on the code has improved it considerably, which is the main reason why I write most of my code as open source.

Not every project I have is abstract math. I also maintain a bunch of code for everything from binding to [OpenGL](http://hackage.haskell.org/package/gl) to performing proper [internationalized hyphenation](http://hackage.haskell.org/package/hyphenation). (For the latter, I really wanted to be able to hyphenate as I word-wrapped error messages in a compiler. It seemed like a good idea at the time!)

### How has the project evolved since you first got involved or first released it?

Lens started out as a small package. It evolved shockingly quickly over the next few months, and reached a very stable point maybe 3 years ago.

As I mentioned above `ad` started out targeted at 4 variables and has been used for everything from high energy physics to movie special effects to robotic motion planning to financial risk analysis.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

Until very recently I probably spent about 80% of my time writing new code. Over the last year or so I've been able to step back a bit and to trust others to deal with many release issues.

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

The Haskell community the nicest group of ridiculously smart people I've been able to find on the Internet. Probably the most frustrating aspect of it all was that it took me a year or two to really figure out how to contribute in a meaningful way. Before I found Haskell I believed that every programming language I learned was really just a matter of figuring out the syntax and few peculiar local idioms. Trying to wrestle with Haskell in that same way was an exercise in futility. People kept telling me that and I just didn't get it.

I love that there always something to learn. But I think the thing that I love most about this community is that it goes out of its way to destroy the notion that there is a dichotomy between the elegant solution and a fast solution. The Haskell community will keep throwing people with PhD's at a problem until they come up with a way to make the elegant solution compile into the fast solution -- and the type system offers enough structure that unlike most other popular languages, these code transformations are possible and safe.

The thing I think most people hate about this community is that there is always something else you feel you HAVE to learn.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

I write a lot of the code that I write to make it impossible to forget a thing. For instance the `ad` library I mentioned above means I can never forget calculus. I have to maintain the library after all, and if a bug shows up now, it is going to be a doozy of a corner case. ;)

I try to let my projects live and die by their own momentum with a few caveats.

One of the things that led me to maintain so many projects in the Haskell community was that I simply couldn't find suitable alternatives maintained by dedicated authors.

Back when I was getting started it seemed like most of the time I'd find a library was either

a.) written by some academic to go with a paper, and was quickly rendered obsolete and unmaintained, because nobody in academia gets paid to maintain old code

b.) written by somebody in industry who was willing to just brute force a solution. They'd maintain it for their own purposes, but they didn't want to deal with large scale breakage to fix up the warts in the API.

I resolved to try to build the boring stuff that wasn't worth publishing and just maintain the damn things. This has proven to be a good recipe for adoption. It also puts a bit of pressure on me to stick around. =)

### What is the most important thing someone submitting an issue or patch should know?

If you're changing a behavior, document why this behavior is better than the alternative.

### What’s your development environment right now?

vim on a macbook with all of about 4 lines of .vimrc:

```
set visualbell
syntax on
colorscheme default
highlight OverLength ctermbg=red ctermfg=white guibg=#592929
```

I tend to write large quantities of code before trying to compile, and I've been using some flavor of vi (badly) for 30 years now.

### What was your first development environment? Do you miss anything from it?

My first development environment was typing in BASIC programs on a Commodore VIC-20. I don't miss much anything about that. My second development environment was an assembler I wrote for the Commodore 64.

The first editor experience that I can actually say I enjoyed was working with Turbo Pascal. By 5.5 or 6, it was ridiculously fast to compile and run code, due to ancient tricks for terminating and staying resident and overlaying code. I often miss that "instantaneous" 1-pass compilation feel.

### Where do you see the open source software community headed?

It seems to be headed in all sorts of directions, all at the same time! Off the top of my head:

BSD-licensed alternatives to many GPL'd projects seem to be finally picking up steam. The GPL is less and less seen as "the default open source license" and more people seem willing to consider more liberal licensing schemes. I think with the GPL projects there to provide a beachhead, there is a lot of room for other strategies to be explored. I personally write a lot of BSD-licensed source code, simply because I want to maximize the number of eyeballs on my code and because I find in general that most companies aren't able to keep up with drinking from the firehose of updates and choose instead to push meaningful contributions back upstream to me rather than try to maintain closed source forks.

My little corner of the Haskell ecosystem is definitely one that prides itself on "correctness" by finding and appealing to mathematics to motivate design where possible. After all category theory has been around for 70 years or so, being thrown at problems from all over mathematics. Not much in the computer science community has that sort of legacy. (FORTRAN and LISP don't engender the same sort of reaction.) This is a bit of a luxury though. Most of the category theoretic concepts we can explore in Haskell can only be given strong types in very few languages. Haskell is fortunate in many ways that it happens to be strong enough to express the bones of these ideas without being so strong that you get bound up in the minutiae of proving every last law.
