---
layout: default
title: "Installing Eclipse and Java for CS320"
---

**NOTE: Always install Java before installing Eclipse**

These instructions are for installing **Eclipse 2020-06** (which is installed on the PCs in KEC 119 and KEC 123).  The instructions will be similar for other versions of Eclipse - but there might be some slight differences.

All of the labs have been reconfigured to use **JRE System Library[JavaSE-1.8]**, which is installed on the PC's in both KEC 119 and KEC 123.  The CS320 labs and example projects will all work with **jre/jdk1.8.0\_301**, which is the specific version of Java that is installed in KEC 119 and KEC 123, along with other earlier versions.  


Installing Java
===============

First, check to see if you have **jdk/jre 1.8.0\_301** already installed, by looking under **C:/Program Files/Java** on your computer.  If so, you can move onto the installation instructions for Eclipse.

If you do not find an acceptable JDK installed on your computer, you'll have to install one from this location:

[Oracle Java SE 8 Downloads](https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html)

Create a free Oracle account and then download and install the appropriate version for your Eclipse/Java installation - the 64-bit version will show up in **C:/Program Files/Java**.

* Scroll down to **Java SE Development Kit 8u301**.

* Now select the appropriate file to download for your operating system.  For Windows-64bit, that will be the Windows x64 Installer: **jdk-8u301-windows-x64.exe**.

* Download the file - it is 169.5MB, it could take a few moments to download.

* Run the executable - it will bring up the installer.  By default, it will install to the **C:/Program Files/Java** folder.  It will install both the JDK and the JRE at that location.

* It is OK to have multiple versions of Java installed on your computer.

Installing Eclipse
=================

After first installing Java, now you can install Eclipse.  We will be using **Eclipse 2020-06** for the CS320 labs (this is the version installed in KEC 119 and KEC 123.

If you already have **Eclipse 2020-06** installed, then you don't need to proceed further. You should attempt to download, import, and install [Lab 2: Web Applications I](./lab02.html) to verify that your installation works.  You might have to tweak the Java version that Eclipse is using.  A link to notes for tweaking your Eclipse/Java installation is included in the Lab02 write-up.

If you need to install Eclipse, you can download the correct version you need for your operating system from this location:

[Download Eclipse IDE for Java Developers: 2020-06](https://www.eclipse.org/downloads/packages/release/2020-06/r)

Installation is simply a matter of unzipping the download into a known location:

  1) For Windows: copy the entire unzipped **eclipse** folder to **C:/**.  You can also have multiple versions of Eclipse installed, just make sure to install them under different folder names, i.e. **C:/eclipse-2020-06/**
  
  2) After unzipping into your chosen folder, go to that folder, and double-click on the **eclipse application**
  
  3) Select a Workspace location: create a folder called **c:/cs320-spring2024**, and then browse to it when prompted
  
  4) Click the Workspace button in the upper right corner after eclipse starts, that will take you to the IDE.
  
  5) Follow the instructions for [Lab 2: Web Applications I](./lab02.html) in order to download and import the **Lab02** and the **Jetty9** server projects into your Workspace so that you can verify that your Eclipse/Java installation works.