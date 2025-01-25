---
layout: default
title: "Lab 2A: Web Applications II"
---

Your Task
===============

**NOTE: This lab will require a significant effort, and you should start on it as soon as possible.**

See [Lab02: Web Applications I Lab](lab02.html) for instructions on how to download the two archive components for Lab02 and then import them into Eclipse.  This version of the lab (Lab02a: Web Applications II) assumes that you have downloaded and completed Lab02 and builds upon the **AddNumbers** and **GuessingGame** examples from that lab.

Lab02a will "force" you to investigate, explore, and learn the structure of a standard WebApp, from **Web.xml**, the servlets, the controllers, the model, all the way through the **JSPs**.  You will need to have this kind of familiarity with the WebApp architecture in order to get started on your team project, as well as to be able to make significant technical contributions to any and all aspects of your team project.  

**NOTE:** You must work individually on this lab.  It is imperative that everyone on your team be able to fully comprehend, design, implement, toubleshoot, and debug the complete architecture of a standard client-server application.  This **WILL** come up on the exam.

**NOTE:** You **are** allowed to use ChatGPT to assist you with this lab.  If you do use ChatGPT, **you must mention it prominently in your comments**.

**NOTE: This lab will require a significant effort, and you should start on it as soon as possible.**

You have six tasks:

* First, make a copy of the **CS320\_Lab02_username** project, and then refactor (rename) that copy to **CS320\_Lab02a\_username**.  YOU MUST DO THIS BEFORE YOU EXPORT YOUR SOLUTION AND SUBMIT IT TO MARMOSET.  **Example:** I would refactor (rename) the copy of my **CS320\_Lab02\_djhake2** project to **CS320\_Lab02a\_djhake2** as soon as I imported the project into Eclipse.  **Submissions that DO NOT adhere to that guideline will not be graded until they are refactored and resubmitted.**

<!-- Commenting out this part - it is too much of a PITA this early in the semester

After you refactor the project name, refactor the package names, change the locations specified in **Web.xml** and the JSP's, as well as the context folder specified in **main()** so that they all refer to **lab02a\_username**. Verify that both of the **AddNumbers** and **GuessingGame** WebApps still work - you will no longer be able to use the URL links included on the **CS320\_Lab02** page, you will need to modify those URLs to replace **lab02** with **lab02a\_username**.  You should save those new URLs as bookmarks in your browser.

-->

* Add a third number to the **AddNumbers** example, such that a third number field shows up on the **AddNumbers** web page, and the returned result is the sum of all three numbers.  Your code should check for the same errors as the existing **AddNumbers** example does.  This problem will require changes to the **AddNumbers** servlet, controller, and JSP.

* Create a new WebApp based on the **AddNumbers** example, called **MultiplyNumbers**.  This WebApp should accept two numbers from the user and return the product of those numbers.  It should check for all of the same errors that the existing **AddNumbers** example does.  This problem will require changes to **Web.xml**, and the controller (modify the existing **AddNumbersController** and refactor it to **NumbersController**, rather than creating a new controller).  You will also need to create a new **MultiplyNumbers** servlet and new **MultiplyNumbers** JSP file, both of which can be based off the **AddNumbers** versions of those files.

* After you have modified **AddNumbers** and created **MultiplyNumbers** and have them both completely working, modify the existing **Index** JSP file so that you can access all three of the servlets (**AddNumbers**, **MultiplyNumbers**, and **GuessingGame**) from the **Index** page.  Implement this as a collection of three "submit" buttons, each labelled with one of the three functions.  Each button will result in **IndexServlet** issuing a **doGet** to the appropriate JSP.

* After all of the above are working, create a common model class (**Numbers.java**) for **AddNumbers** and **MultiplyNumbers**, such that the numbers submitted through the HTTP request are stored in the model, along with the result.  You will need **get** and **set** accessor methods for all model fields, along with a constructor for the model class.  Look at the model for the **GuessingGame** WebApp as a template - and how that model is instantiated, initialized, and accessed.  The corresponding JSP's should pull the data directly from the **Numbers** model, rather than from the HTTP request.  Again you can look at the **GuessingGame** implementation to see how this is done.

* As part of this exercise, implement a complete set of test cases for the controller and model classes.  Implement those test cases as you develop each of the above tasks.  A significant portion of the effort on your team project will be creating an extensive and comprehensive set of JUnit test cases - **WHILE YOU ARE DEVELOPING YOUR TEAM PROJECT**.

**NOTE: I HIGHLY recommend that you save your work after you have each of the above steps working.**  To that point, I also highly recommend that you use this lab as a means for learning how to use **git** to store your changes on **GitHub**.

*	At a minimum, archive the project at each stage, and submit it to Marmoset.  That will provide a back-up in case you lose your work, or if you need to revert to a previous version of your work.
*	If you want to keep your previous work accessible to you, make copies of your project in Eclipse after the completion of each step, and then rename that copy to indicate the completed step.  Continue your effort in the existing project.
*	I still **strongly** suggest regularly storing your archives to Marmoset (preferably to GitHub) so that you can restore your work if your PC dies.

**NOTE:** You must work individually on this lab.  It is imperative that everyone on your team be able to fully comprehend, design, implement, toubleshoot, and debug the complete architecture of a standard client-server application.  This **WILL** come up on the exam.

Submitting
==========

**NOTE:** You must also get this lab signed off by a tutor/mentor or your instructor in order to get credit for it.  Simply submitting the lab to Marmoset without a lab sign-off will **NOT** result in any credit.  **You must get a lab sign-off**.

**[Here is the complete set of tests that will be used to sign-off on your lab.](lab02a-signoff-criteria.html)**

Here is a [PDF version of the complete sign-off criteria](CS320-Lab02a-WebApplicationsII-LabSignOff.pdf) that you can **download, print, and use as a checkoff list when you get the sign-off for the lab.**

Although you should strive to satisfy all of the above tests, a minimum passing submission must have the following:
* An **operational Index page** that links to all 3 applications
* The **Add Numbers page** must allow entry of three numbers
* A **Numbers.java** model file
* **AddNumbers.JSP** and **MultiplyNumbers.JSP** must pull their field data directly from **Numbers.java** and **NOT** from the original parameter values passed in through the HTTP POST received by the Servlet.
* There will be at least **some test cases** for the methods in **NumbersController.java** and **Numbers.java**

When you are done, submit the lab to the Marmoset server using the method below.

From a web browser
------------------

Save your project (**CS320\_Lab02a\_username**) to a zip file by right-clicking it and choosing

> **Export &rarr; General &rarr; Archive File**

Make sure to choose an appropriate location and archive name before saving the archive, or you might unintentionally overwrite an archive that you previously saved.

Upload the saved zip file to the **Lab02a** project on the Marmoset server. The server URL is

> [https://cs.ycp.edu/marmoset/](https://cs.ycp.edu/marmoset/)


