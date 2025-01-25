---
layout: default
title: "Lecture 6: Software Development Processes"
---

Development Processes
===================

[From Chapter 2 in UML Distilled]

A development process is a structured collection of practices and guidelines that all team members follow.

At the beginning of the process, we start with a "word problem" that we (you, your team, your client(s), and/or your company) want/need you and your team to solve.

At the "end" of the process, we have a finished system that fulfils the requirements for the project.

"End" is a bit misleading; typically, the software we develop will be continuously modified and extended. It's more accurate to say that at some point, the software will be deployed and officially "in-use".  Development/improvement will likely continue after each release of the project.

Having a defined process helps the members of the team work together.

Two of the most-widely-used software development processes are **Waterfall** and **Iterative, AKA Agile**.

The **Waterfall** process is intended to be a single iteration through the following phases:

> Requirements → Analysis → Design → Implementation → Testing → Deployment (Release)

An **Iterative** process is a series of short iterations (2-4 weeks), each of which is a "mini-waterfall" process, with a release at the end of each iteration.  We will discuss the iterative process in the next lecture.

Waterfall Process
-----------------

The **Waterfall** process can be easy to understand, and might sound attractive in theory because it ostensibly provides a high level of determinism in relation to project scheduling, required resources, and overall cost and development time.  Upper-level management tends to find the Waterfall process attractive due to its "mythical" allure for that determinism.  In reality, however, the Waterfall model is both impractical and too inflexible since there is no opportunity for feedback and intermediate iteration during the process.

For example, we may (and most likely will) discover new requirements during the Analysis phase, we may (and most likely will) discover more about the problem during the Design phase, etc.   And those discoveries will cause an iterative jump further back in the process.

Another major weakness of the Waterfall model is that estimation is very complex: it's extremely difficult to predict how long we will need to complete each stage. It is also risky to assume that the entire system will "come together" at the end of the Implementation phase.

Let's work through an example of an actual project implemented using the Waterfall process and discuss where the failure mechanisms can (and do) arise.  