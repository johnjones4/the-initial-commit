---
layout: post
title: "Alexis de Talhouët"
image: "alexis.jpg"
seo_title: "An Interview With OpenDaylight's Alexis de Talhouët"
description: "I work mostly on the OpenDaylight project, maintaining many sub-projects it has, with a high amount of focus on the core projects."
links:
  - name: github.com/adetalhouet
    url: https://github.com/adetalhouet
  - name: www.adetalhouet.com
    url: http://www.adetalhouet.com/
projects:
  - name: OpenDaylight
    link: https://www.opendaylight.org/
---

### What project or projects do you maintain and what was your motivation for creating those projects and releasing them as open source software?

I work mostly on the OpenDaylight project, maintaining many sub-projects it has, with a high amount of focus on the core projects. OpenDaylight is a framework providing tools to build software-defined networking (SDN) controllers. Core projects are the ones providing the data store, the underlying communication with the data store (using NETCONF/YANG), and everything related to clustering that leverages Akka framework for inter-node communication.

First, I think the motivation comes along with the current trend in Open Networking and all of the Open Standards that are being established. I'm a true believer in Open Source communities and the meritocracy they are based on. Second, working within Open Source communities is the best way to learn fast and keep up-to-date on many new technologies being developed. Open Source contributors persistently lead on developing new innovative technologies and are full of knowledge, eager to help, and provide good insight and best practices. For me, picking their brain is a good way, as an autodidact, to learn and improve.

### If you created any of those projects, were they meant to solve a specific problem you faced, or were they born out of a larger opportunity you saw?

All the projects I have been part of since their inception, were meant to solve specific problems that were highlighted either within the community or driven by a customer engagement and/or customer needs.

I haven't yet got the opportunity to create a project from scratch that potentially aims to provide a large framework, a base or a de facto standard to be used/re-used by everyone, but this is something I aim to accomplish someday.

### How has the project evolved since you first got involved or first released it?

I joined the OpenDaylight community during the early third release, and have since been a day-to-day contributor. I'm seeing major improvements on important topics such as clustering, high availability, scalability of southbound protocols and longevity. For an SDN controller, it is important that it scales properly, by maintaining a stable environment that avoids any in-service disruption.

### How do you spend your time on those projects? (i.e. Developing, managing the community, triaging issues, etc.)

I spend my time maintaining the projects, keeping them up-to-date, reflecting best practices, and ensuring inter-project consistency. Also, I try to be as active as possible on mailing-lists to answer anyone's needs, questions, and on the question/response platform the project has. Finally, I spend some time reviewing submitted code and provide some reviews when the patch is in my range of expertise.

### How would you describe the community around projects you participate in? What are your favourite and least favourite aspects?

The community is always welcoming with regards to the code you push within their project. Push a patch and you'll get a review, as long as you add the appropriate reviewers to it, of course. Also, having weekly meeting and mailing-lists help us communicate and strive for agreements on new functionalities, and how to implement them, or what and how to address open bugs.

My favourite aspect is that the community is worldwide, hence, at any time you have some commitment happening. Sometimes it's too much commitment and begins to get difficult to follow and sometimes committers of the projects are in the same time zone, which can slow down the review process.

### What keeps you involved in those projects? Do you have long-term plans for maintaining your involvement?

My involvement is mostly driven by my interest in the domain the projects co-exist, which is the networking domain. I'm planning on being involved as long as the projects have users, and my day-to-day job at Inocybe Technologies enables me to deliver these projects or more specifically, lessening the barrier to organizations using them.

### What is the most important thing someone submitting an issue or patch should know?

When you open a bug/ticket/jira/issue, whatever you call it, you must always provide the following:

* version
* component
* environment
* expected vs observed
* step-to-reproduce
* stack trace
* logs (set at the DEBUG level if possible)

Those elements will allow the developer picking up the issue to accurately assess it to be able to scope it correctly.

When submitting a patch, one should systematically provide unit test along with the added source code. If you're modifying or adding a new functionality, you should also provide some documentation on how it is intended to be used.

Also, be aware of the project licensing and best practices to follow its conventions and reduce the back-and-forth.

### What’s your development environment right now?

Macbook Pro 15'

IntelliJ IDEA 2016.3

Terminal, TextMate on OSX

Solarized color theme for Terminal, IntelliJ, IRC

I was an Eclipse fan and switched to IntelliJ a couple of months ago. I struggle to go back to Eclipse, but I still use it from time-to-time as I have things specifically setup to work only with Eclipse.

### What was your first development environment? Do you miss anything from it?

It was my 13' Macbook Pro that I bought as a student. The laptop on which I built my first Android/iOS apps back in the day. I don't miss anything about it as I still use a Macbook Pro, although my new Macbook has way better performance. On my old Macbook, I wasn't able to run more than a VM. Now I can run many VMs and containers at the same time, while the laptop is still fast and responsive. Good progress was made in this area.

### Where do you see the open source software community headed?

Open Source software is becoming a de facto standard in the networking industry. Everyone involved in this industry wants to leverage Open Source components, mostly hosted by The Linux Foundation. I see the OSS community evolving and working even more together to be able to provide next generation technologies, setting the acceptance criteria higher and reducing vendor lock in and/or proprietary software. To be more precise, I believe all proprietary software will soon be based on Open Source components, making that software more interoperable.
