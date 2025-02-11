---
layout: default
title: "Installing Eclipse and Java for CS320"
---

**NOTE: Always install Java before installing Eclipse**

These instructions are for installing **Eclipse 2024-12 IDE for Enterprise Java and Web Developers** (which will also be installed on the PCs in KEC 119 and KEC 123).  The instructions will be similar for other versions of Eclipse - but there might be some slight differences.

All of the CS320 labs have been reconfigured to use **Eclipse Temurin builds of OpenJDK 8** (which replicates Oracle Java JRE/JDK 8).  This open source option includes both OpenJDK 8 and the corresponding JRE, and can be found at [Eclipse Termurin Open JDK 8](https://adoptium.net/temurin/releases/?version=8&os=windows).  OpenJDK 8 will also eventually be installed on the PC's in both KEC 119 and KEC 123.  The CS320 labs and example projects will all work with **OpenJDK 8**.

**NOTE:** Make sure to install the **OpenJDK 8** version from above, as the CS320 labs might not work with other versions of Java.  


Installing Java
===============

First, check to see if you have **jdk-8.0.442.6-hotspot** already installed (unlikely), by looking under **C:/Eclipse Adoptium** on your computer.  If so, you can move on to the installation instructions for Eclipse.

If you do not find the above OpenJDK 8 installation on your computer, you'll have to install it from [Adoptium Temurin Open JDK 8](https://adoptium.net/temurin/releases/?version=8&os=windows).

Follow the link above, which takes you directly to the **Temurin 8.0.442+6** release.  Select your operating system (it defaults to Windows) and download the appropriate version for your operating system.

* **Windows:** Download the **x64 JDK .msi file** (the top entry shown).

* **macOS:** Download either **x64 JDK .pkg or x64 JDK .tar.gz** (one of the top 2 entries).  See Dr. Babcock for details.

* **Linux:** Download the JDK version appropriate for your hardware configuration.  See Dr. Babcock for details.

After downloading the file, install the JDK package (all downloads are around 100MB, which could take a few moments to download).

* **Windows:** Double click on the **.msi** file that was downloaded.  By default, it will install to **C:/Eclipse Adoptium/jdk-8.0.442.6-hotspot**.  It will install both the JDK and the JRE.

* **macOS:** TODO for Dr. Babcock

* **Linux:** TODO for Dr Babcock


Installing Eclipse
=================

After first installing Java, now you can install Eclipse.  We will be using **Eclipse 2024-12 IDE for Enterprise Java and Web Developers** for the CS320 labs and for your team project (this is also the version to be installed in KEC 119 and KEC 123.

If you already have **Eclipse 2024-12** installed, then you don't need to proceed further. You should attempt to download, import, and install [Lab 2: Web Applications I](./lab02.html) to verify that your installation works.  You might have to tweak the Java version that Eclipse is using.  A link to notes for tweaking your Eclipse/Java installation is included in the Lab02 write-up.

If you need to install **Eclipse 2024-12**, you can download the appropriate version you'll need for your operating system from [Download Eclipse IDE for Enterprise Java and Web Developers: 2024-12](https://www.eclipse.org/downloads/packages/release/2024-12/r/eclipse-ide-enterprise-java-and-web-developers).  Select the download approproate for your operating system.

Installation is simply a matter of unzipping the download into a known location.  Create an **Eclipse-2024-12** folder on your home drive (**C:/ for Windows**):

  1) Copy the entire unzipped **eclipse-jee-2024-R...** folder to your **Eclipse-2024-12** folder.  This allows you to maintain multiple different Eclipse installations.
  
  2) After unzipping into your chosen folder, go to that folder, and double-click on the **eclipse.exe** application file.  Eclipse will start up.
  
  3) Select a Workspace location: create a folder on your home drive called **cs320-spring2025**, and then browse to it when prompted for a Workspace.  You will use this workspace for all of your labs.  You will eventually create a separate workspace for your team project.
  
  4) Click the Workspace button in the upper right corner after Eclipse starts, which will take you to the IDE.
  
  5) Follow the instructions for [Lab 2: Web Applications I](./lab02.html) in order to download and import the **Lab02** and the **Jetty9** server projects into your Workspace so that you can verify that your Eclipse/Java installation works.