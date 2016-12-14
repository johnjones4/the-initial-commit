---
layout: post
title: "Federico Mena Quintero"
seo_title: "An Interview With Gnome's Federico Mena Quintero"
description: "Currently I only maintain librsvg, a small library to render SVG files - GNOME uses it to render icons in applications, for example, and Wikimedia uses it for the scalable diagrams in Wikipedia pages."
links:
  - name: github.com/federicomenaquintero
    url: https://github.com/federicomenaquintero
  - name: people.gnome.org/~federico/news.html
    url: https://people.gnome.org/~federico/news.html
projects:
  - name: librsvg
    link: https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg
tags: ["gnome"]
---


### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

Currently I only maintain librsvg, a small library to render SVG files - GNOME
uses it to render icons in applications, for example, and Wikimedia uses it for
the scalable diagrams in Wikipedia pages.

I didn't create librsvg.  It has been the product of many years of work
by several people in the GNOME project.  I think librsvg started
during the days of Eazel; the ChangeLog goes back to 2001.  I'm just
the current maintainer; it happened because the project was effectively
unmaintained, and some people asked if I could take care of it.  I had
done some bug fixes to librsvg in the past, so I agreed to it.

In GNOME I've maintained different things over the years; I didn't
create all of them.

Of the ones I did create and maintained, my motivation was the same as
for the rest of GNOME:  because I agree with the FSF's motivation for
free software.  I also agree with the "secondary" derivations of the
four freedoms:  I live in Mexico, where proprietary software is
terribly expensive and always seems to come from other countries, so it
doesn't help ours.  I like that free software can be made more secure
and trustworthy than proprietary software.  I also like "giving back"
to the free software commons at large, since I have gotten so many
things out of it.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

I've created a number of things over the years:

gnome-panel was one of the very first GNOME modules; it displayed the
bar at the bottom of the screen with several utility applets and
application launchers.  We needed it to have a "complete" desktop as it
was perceived back then.  It also gave me an excuse to learn how to
write a plugin system from scratch.  Gnome-panel doesn't exist as such
anymore; it got replaced with Gnome-shell.  I am not sure if the Mate
desktop still uses gnome-panel code.

gnome-canvas was a programming library for retained-mode 2D drawing.
My friend Miguel de Icaza convinced me that having something like that
would make it easier for people to write graphics-rich applications in
GNOME, so I ported the Tk Canvas to GTK+ and added some extra
functionality.  It worked very well for its time!  And it did provide
us with graphics-rich applications.  It is not really used anymore, but
applications like Inkscape and Ardour still use drawing engines based
on gnome-canvas.

EOG (Eye of Gnome) is an image viewer.  That one was to scratch an
itch of my own:  I liked downloading large images from satellite
photos, but had no good way to view them.  In 1998 or '99, image
viewers for Linux just weren't very good at displaying large images and
letting you zoom and pan around them.  I saw a proprietary image
viewer, called Compupic, that did a pretty stellar job of this, and
that was my inspiration.

Mortadelo was more or less an equivalent to the Windows utility
Filemon.  It was a tool to monitor all the system calls done by all
programs in a system.  At Novell we had a customer request where
someone, possibly a former Windows sysadmin, wanted something like
Filemon but for Linux.  So, I wrote Mortadelo using Systemtap as a
backend.  I wish someone would resurrect it, but using some of the
newer tracing features in the Linux kernel.

La Mapería is a script to create beautiful printed maps from
OpenStreetMap data.  I like cartography, and cycling around the
mountains in my region, and I wanted good topographic maps.

But mostly, I've inherited the maintenance of other things, rather than
having created them myself.  You know when you move into a house,
maintain it for a few years, make a few changes here and there, and
then move to another place?  It's very much like that.

### How has the project evolved since you first got involved or first released it?

Librsvg, you mean?  Let me tell you!

Librsvg has passed through several maintainers; I'm just the latest
one.  I inherited it when some bug fixes had piled up, but no one had
made a release for some time.  In GNOME, unfortunately, we have some
pieces of infrastructure that are kind-of-but-not-really maintained
like that:  some kind soul integrates patches every now and then and
makes a release, but they don't really continue development on that
infrastructure.

I was doing the same for librsvg until a few weeks ago, when I decided
to learn the Rust programming language - a safe, modern, systems
programming language.  Librsvg is written in C, an old, unsafe, systems
language.  I started porting bits of it to Rust, and now librsvg is
like a somewhat forgotten garden that is flowering again.  The code
structure is getting better; we have a much improved test suite; we
have some safe Rust code to replace some potentially unsafe C code.

My intention is that this will give people an example of how to port
our GNOME infrastructure from C to Rust, to make it safer and easier
for the future.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

Oh, it varies a lot, depending on the project.  Currently librsvg is a
one-person shop, but hopefully I can find some Rust people who are
interested in computer graphics to help

### How would you describe the community around projects you participate in? What are your favorite and least favorite aspects?

GNOME is a large community, with a bunch of volunteers and a bunch of
dedicated companies participating.  I like the opportunities that "the
free desktop" presents to various kinds of people:

For casual participants, it is a good way to work on very visible,
general-purpose infrastructure instead of an obscure app.  It's like
being able to put up benches and flower planters in the city's main
square, instead of just embellishing a shop somewhere.

For companies, it's a great, trustworthy desktop that they can ship.
 Developing a graphical environment takes rather monumental amounts of
work, and GNOME is just there and it works.

For government/school/company deployments, GNOME provides a system
that has been tested to be actually usable by non-technical people.
This reduces support costs for them.

My favorite aspect is being able to hop from one of these opportunities
to another.  Sometimes I like doing infrastructure work; other times I
like attacking horizontal problems across the platform.  Sometimes I
like to engage with users, etc.

My least favorite aspect is getting myself distracted with so many
options!

### What keeps you involved in those projects? Do you have long term plans for maintaining your involvement?

Well, GNOME pays my salary.  Okay, not the GNOME project directly, but
Suse, my employer, pays me to work on GNOME.  So, you could say that I
have a vested interest in keeping myself involved.

### What is the most important thing someone submitting an issue or patch should know?

Every maintainer of GNOME's sub-projects has their own preferred way of
working.  Someone who submits a patch should make themselves familiar
with that way of working, and accomodate the maintainer - some prefer
patches being sent to our bug tracker; others may prefer discussing
things on a mailing list, or getting a pull request somewhere.

It helps a lot for patch submitters to make it as easy as possible for
maintainers to evaluate their patches.  Do they follow the source
code's indentation style?  Do they have tests?  What sort of research
was done to write this patch?

### What’s your development environment right now?

I have a fast desktop PC which sits on the floor, a good monitor that I
wish had more pixels, a *fantastic* old full-travel keyboard, and a
wired Microsoft mouse which is nice and clicky.  I have a second
desktop PC with a smaller monitor which is my "non-work" machine, but
which does double-duty as my documentation-reading machine while I do
work on the other one.

I have a not-too-fancy laptop which mostly accompanies me to the
toilet.  Don't ask, you already know what I'm talking about.  I don't
travel much these days, but that's my development machine while on the
road, too.

I'm an old fogey who uses Emacs and GNU Screen inside a terminal window
instead of an IDE.  Emacs has gotten incredible in the past few years,
and my fingers are too accustomed to it now to try something else.  I
understand that it is not everyone's favorite environment, though.

### What was your first development environment? Do you miss anything from it?

Pretty much the same as it is now, except with a 80486SX CPU. I
really miss nothing from it, except for the quietness.  Remember when
fan noise was not a consideration?

### Where do you see the open source software community headed?

There are some very interesting things going on:

Flatpak and similar ways to ship applications are making it easier
for people to get their apps to end users.  Currently, Linux
distributions are an uncomfortable intermediary.  Also, Flatpak would
make it easier to have app stores where users can actually give money
to application authors.  Which brings me to...

Efforts by people like The Recompiler Magazine's editors to figure
out a way to make it possible for people to earn a living from writing
free software.  If you are not paid by a free software company, it is
really hard to make a living.  It is also very hard to make a company
just to support an app.  We are unfortunately plugged and woven into
the capitalist system, where money is required to survive.  It is odd
that free-as-in-freedom software has not really been concerned with its
own economic sustainability.

The worldwide realization that governments are not to be trusted in
the digital space.  People are starting to distrust proprietary or
state-sanctioned software, and this is a huge opportunity for free
software if we can manage to become economically sustainable.
