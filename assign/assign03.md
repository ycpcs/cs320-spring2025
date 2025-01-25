---
layout: default
title: "Assignment 3: Team Project Milestones"
---

In the [Schedule](../schedule.html) you will notice days designated as team project milestones.  These are opportunities for your group to demonstrate progress on your team project.

This document describes the expectations for each milestone.  See the [Assignment Schedule](./index.html) for actual due dates.

> Assignment | Milestone
> ---------- | ---------
> Assignment 3a      | Milestone 1: Minimal Working System (Basic navigation)
> Assignment 3b      | Milestone 2: Progress on Features (interaction with fake database)
> Assignment 3c      | Milestone 3: 75% Working System (operational persistent SQL database)
> Assignment 8a      | Final Technical Report - submit in PDF form to Marmoset
> Assignment 8b      | Final Presentation & Demo, during final exam period

## General Milestone Expectations
Each milestone will be a **formal** presentation, where your team should be assembling a collection of 5-10 PowerPoint slides, **along with a demonstration of your working code, and a run of the complete set of test cases that you have developed to that point.**  Bear in mind that it is acceptable for **some** of your test cases to fail, as you will not have implemented all of your code - at least for the first three (3) milestones above.

**Slides to consider (you may include others, as you see fit):**
* Project title slide that also includes all of the names of the team members.
* Brief description of you project.
* Updated version of your UML diagram.
* Updated version of your database schema - all DB tables with all attributes and their respective data types for each table (NOT required for Milestone 1, required for Milestone 2 for the Fake database).
* List of major features, with the status of each feature.
* Task assignments for the team members.
* Challenges you have encountered, and how you have dealt with them.
* Goals for the next milestone.

**Following your slide presentation:**
* Demonstrate the current functionality of your project.
* Run your suite of test cases.


## Specfic Milestone Expectations
**Milestone 1: Minimal Working System**. Your team should demonstrate:

* A web-based user interface (e.g., JSPs and servlets) that implements a small number of essential features in some minimal form: provide as much navigation between pages as you can
* Model classes, controllers, and unit tests associated with a small number of "essential" requirements
* A persistence interface and a "fake" in-memory implementation of the persistence interface (e.g., using array lists to store model objects rather than database tables)
* For this milestone, if you want to persist user-entered data between your UI and your server, consider using the HTTP Session for that.

The idea of a minimal working system is to create a working foundation early in the project's development.  Subsequent iterations of the development process will build upon this foundation to implement additional features.

**NOTE: Please assign your instructor as a contributor to your main Team Project Repository on GitHub, and email a link to your Repository to your instructor, BEFORE your Milestone 1 presentation.**

**NOTE: In order to hit the first milestone, and place your team in a good position to achieve success, you will need to put in a good deal of initial development work on your web front-end navigation before and over Winter Break.**

**Milestone 2: Progress on features**.  In this milestone, your team should demonstrate some progress on features, such that at least some use cases are fully or partially implemented.  It is fine if your system is still using the "fake" database at this point.  For this milestone, if you want to persist user-entered data between your UI and your server, consider using the HTTP Session for that.

**Milestone 3: "75%" Working System, Persistence using SQL database**. Your team should demonstrate a working system that implements most of the major system requirements.  Also, Your team should demonstrate that there is a working implementation of the persistence interface that uses an SQL database to store and retrieve data (e.g., using Derby).  Note that it is not expected that the system has a high degree of "polish": the UI doesn't have to be beautiful, for example.  However, the features that are implemented should be functional and free of bugs.  Make sure to include the following slide in your presentation (in addition to your other slides):

* A slide on your SQL database schema, which should include your tables, the attributes in each table and their data types, and any relationships between the tables.  You can use the format shown in [Lecture 13](../lectures/lecture13.html) for your tables.  You do NOT need to include any actual data in the tables, unless it is for explantory purposes.

* A slide that lists the names of your SQL database methods (queries, inserts, updates, etc.)  Note that this should NOT include the SQL code, but rather method names, such as "getAllBooksByAuthor()", along with a short description of each method.  This will be a list of the DB methods that you have included in your IDatabase interface.

* A slide summarizing the current progress on your project, i.e., a list of features that have been implemented.

* A slide summarizing the major technical challenges that your team faced, and how you overcame them.

* A slide summarizing what you plan to accomplish before your final presentation and demo.

## Evaluation

For each of these milestones, I will give your team one of the following grades: *below expectations*, *meets expectations*, or *exceeds expectations*. Below expectations means that I am concerned that your team is not making sufficient progress.  At all 3 milestones, I expect that there will be sufficient effort put towards automated unit test case development.

<div class="callout">
<b>DO NOT LEAVE TEST CASES AS AN AFTER-THOUGHT.  YOUR TEAM WILL RECEIVE "BELOW EXPECTATIONS" IF YOU DO NOT HAVE SUFFICIENT TEST CASES DEVELOPED FOR EACH MILESTONE.</b>
</div>