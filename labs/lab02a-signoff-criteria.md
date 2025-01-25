---
layout: default
title: "Lab02a: Web Applications II Lab Sign-Off"
---

Tests for Web Applications II Lab (Lab02a) Sign-Off
===============
 1) Pull up **Lab02a** in Eclipse: Verify project name has been changed to **"CS320\_lab02a\_username"**, "username" = student's YCP username.

 2) Pull up **Index page**: Verify that the there are links/buttons for **AddNumbers**, **MultiplyNumbers**, and **GuessingGame**.

 3) Go to **Add Numbers** from **Index page**: **AddNumbers** page appears, with three number fields.

 4) Enter **three numbers**: Get correct sum.
 
 5) Delete **third number**: Get correct error message: **"Please enter 3 numbers"** (required), fields have original values (extra credit).
 
 6) Replace **third number** with **"abc"**: Get correct error message: **"Invalid double"** (required), fields have original values (extra credit).

 7) Go back to the **Index Page**.

 8) Go to **Multiply Numbers**: **MultiplyNumbers** page appears, with two number fields.
 
 9) Enter **two numbers**: Get correct product.
 
10) Delete **first number**: Get correct error message: **"Please enter 2 numbers"** (required), all fields have original values (extra credit).

11) Replace **first number** with **"abc"**: Get correct error message: **"Invalid double"** (required), all fields have original values (extra credit).

12) Go back to **Index Page**.

13) Go to **Guessing Game**: **GuessingGame** page appears, **"Start Game"** displayed.

14) Use **33** as the number: Press correct buttons, application eventually guesses 33.  Sequence of guesses: **50** -> **25** -> **37** -> **31** -> **34** -> **32** -> **33**.

15) Pull up **Numbers.java**: Verify encapsulation.  Model attributes are private, and public constructor(s), getters, setters have been provided.

16) Pull up **addNumbersServlet.java**: Verify **ONLY** **error message** and **model** paramters are being set in the HTTP request.

17) In **addNumbersServlet.java**: Verify MVC is followed.  **NO** direct calls to **Numbers** model setter methods.  Only controller methods used to change**Numbers** attributes.

18) In **multiplyNumbersServlet.java**: Verify MVC is followed.  **NO** direct calls to **Numbers** model setter methods.  Only controller methods used to change **Numbers** attributes.

19) Pull up **addNumbers.JSP**: Verify it **ONLY** pulls model data directly from **Numbers.java** model.

20) Run JUnit tests for **NumbersController.java** and **Numbers.java** methods: Test cases exist and pass.  Complete test cases cover **constructor(s)**, **getters**, **setter(s)**, and **add** and **multiply** methods.