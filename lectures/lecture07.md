---
layout: default
title: "Lecture 7: Agile & Scrum"
---

Iterative Development process
=============================
As we've seen, the **Waterfall process** can be easy to understand, and might sound attractive in theory because it ostensibly provides a high level of determinism in relation to project scheduling, required resources, and overall cost and development time.

Hoever, we discussed the risks and downfalls of the Waterfall process in the [previous lecture](lecture06.html).

The overall goal in an **Iterative** process is to make sure that the software is always in a consistent, stable state. At the end of each iteration, we should have a correctly working system that achieves a (hopefully) increasing subset of the current requirements.  We can then demonstrate steady progress (at any time) by running the most recent working version of the application.

Keeping the iterations short makes estimation and planning easier: we can get a pretty good idea of the rate of progress by seeing (on average) what % of the requirements we can finish at the end of each iteration

The risk of trying to **integrate** (put together) the entire system and test it at the end of the **Waterfall** process is mitigated via an **Iterative** process because the software is in a high-quality and tested, "ready to deploy" state at all times.

Another important characteristic of a process is the level of **ceremony**. A **high-ceremony** process is one in which each development activity is done in a very specific way, and where the design artifacts (documentation) created at each step (use cases, functional specifications, analysis and design models, etc.) may be highly detailed. A high-ceremony process may be necessary if the system being developed is safety-critical (medical devices, weapons, spacecraft, avionics, etc.)

For many projects, a lower-ceremony process probably makes more sense.

Agile Processes
---------------

Agile is a form of iterative process - a series of short iterations (2-4 weeks), each of which is a "mini-waterfall".  Agile is a good general choice for non-safety-critical projects because it's low-ceremony and it emphasizes:

-   incremental development
-   direct and continuous interaction with clients/customers
-   adapting to changing requirements by keeping the software flexible

Here is a sketch of what working within an agile process might look like.

> <img style="width: 700px;" src="figures/xpProcess.png" />

The client/customer is in constant contact with the development team, and is continually

-   explaining requirements (including changes and/or additions to requirements)
-   prioritizing requirements

At the beginning of each iteration or **sprint** (let's say we will have two week sprints), the customer chooses a set of requirements to be addressed in that sprint, in order from most important to least important. The requirements are recorded as **Use Cases** (how the User will use the application).

The developers take the Use Cases, and use them to update the **Aanalysis and Design Models**. That step is necessary because the existing design may not have anticipated the requirement being addressed by the Use Case, and needs to be extended to address the requirement. If the Design Mndel changes, the code usually must be refactored to conform to the new Design. Refactoring means changing the internal structure of code without changing WHAT the code does. In other words, after refactoring a program, the functionality of the program is exactly the same.

Examples of refactoring:

-   Moving a method from one class to another
-	Splitting a method into multiple methods
-   Moving a field from one class to another
-   Splitting a single class into two classes
-   Splitting a single class into a class hierarchy (superclass and subclasses)

As developers refactor the code, they run all of the **Automated Unit Tests** to make sure that the refactoring does not introduce any new bugs. Unit Tests are low-level (fine-grained) tests that check whether particular classes/methods work correctly. The refactoring is complete when

-   the code matches the updated design
-   all of the pre-existing unit tests pass

Once refactoring is complete, the developers modify the code to add new features (addressing the requirements selected by the customer for the sprint). As they work, the developers also develop the associated unit tests to ensure the new classes and methods they are adding work correctly, and continue to run the old unit tests to make sure that no **regressions** have been introduced. A regression is a bug in which a change to the code causes a feature that previously worked to no longer work correctly.

At the end of the spring, the developers have implemented some number of new requirements.

If all of the customer's chosen requirements for the week have been addressed, great. Everyone's happy.

If some of the customer's chosen requrements have not been addressed, then the schedule has slipped. This is not necessarily bad; some aspect of a requirement may have been more complicated than anticipated. The customer and the development team adjust their planning appropriately. Occasional schedule slips may be tolerated. Frequent schedule slips mean that the developers are overestimating their rate of progress, and need to avoid over-committing in future increments.

The accumulation of schedule slips (meaning that a feature was not fully incorporated for a given sprint) and unaddressed bugs becomes the **backlog** of work for the project.  Issues on the backlog will need to be fit into future sprints, which tends to push out schedule work.  Ideally the backlog should be shrinking.

There are a lot of good things about agile processes:

-   The rate of progress is always apparent - no big surprises.
-   Changing requirements are handled more easily (or with less difficult, depending on the point of view).
-   The customer is always "in the loop" and decides what work will be done. Developers don't spend time implementing unnecessary features. The most important features are the ones implemented first.
-   The system remains in a "ready to deploy" state at all times. (It might not implement all required features, but the features that are implemented work correctly.)

Let's take a look at some examples of what an agile development sprint schedule looks like and how it leads to incremental improvements in application functionality.

- [CS201: Disk Game](https://ycpcs.github.io/cs201-fall2021/assign/assign01.html)

- [CS320: Web Applications Lab02a](../labs/lab02a.hml)