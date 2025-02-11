---
layout: default
title: "Notes for Lab 2: Guessing Game WebApp"
---

Determining the JRE System Library
==================================

These instructions are for **Eclipse 2024-12 IDE for Enterprise Java and Web Developers** (which will be installed on the PCs in KEC 119 and KEC 123).  The instructions will be similar for other versions of Eclipse - but there might be some slight differences.

All of the CS320 labs have been reconfigured to use **Eclipse Temurin builds of OpenJDK 8** (which replicates Oracle Java JRE/JDK 8).  This open source option includes both OpenJDK 8 and the corresponding JRE, and can be found at [Eclipse Termurin Open JDK 8](https://adoptium.net/temurin/releases/?version=8&os=windows).

OpenJDK 8 will also eventually be installed on the PC's in both KEC 119 and KEC 123.  The CS320 labs and example projects will all work with **OpenJDK 8**.

All of the labs will be reconfigured to use **jdk-8.0.442.6-hotspot**, which will be installed on the PC's in both KEC 119 and KEC 123.  It is possible that the configuration you are using on your own PC (or even on a lab PC) could vary such that the OpenSource JDK 8 cannot be found.  The instructions below will help you establish the proper JRE System Libraries for the labs for CS320.

If you are using a different version of the **JRE System Library** with Eclipse 2024-12, you should change the default **JRE System Library** version to **jdk-8.0.442.6-hotspot** in order to get **CS320\_Lab02** to work.

* Create a folder named **cs320-spring2025** on your own PC's home drive (C:/ for Windows) and/or your YCP home drive **(H:)**.

* Create a sub-folder called **archives** within that **cs320-spring2025** folder for storing your download archives and your lab submission archives.

* Set the **Default Workspace** for Eclipse 2024-12 to the **cs320-spring2025** folder.

* Download **CS320\_Jetty9.zip** and **CS320\_Lab02.zip**.

* Open Eclipse 2024-12, switch the **Workspace** to **/cs320-spring2025** (on the home drive of your own PC) or **H:/cs320-spring2025** (on a lab PC).

* Import **CS320\_Jetty9.zip**.

* Import **CS320\_Lab02.zip**.

* Expand both projects.

* If each project shows the **JRE System Library** as **jdk-1.8.0.442.6-hotspot**, then you likely have no further steps to take.  You can start to work on **CS320\_Lab02**.

Changing the JRE System Library
===============================

On the other hand, if the **JRE System Library** is shown as a different JRE/JDK or is "unbound", you will need to switch to a compatible library.

Assuming that you have downloaded and installed **jdk-1.0.8.442.6-hotspot**, go to **C:/Program Files/Eclipse Adoptium**.  There should be a folder named **jdk-1.0.8.442.6-hotspot**.

It is possible that there are other versions of Java installed under the **C:/Program Files/Java** folder.  Those are **NOT** the Java versions we are looking for.

* Go into Eclipse, right-click on the **CS320\_Lab02** project.

* Go to the the bottom, select **Properties**.

* Select **Java Build Path** on the left.

* Select the **Libraries** tab.

* Select the **JRE System Library** entry.

* Select the **Edit...** button on the right.

* Select the **Installed JREs...** button on the right.

* That will pop up a list of installed JRE's.

* If you see one for **jdk-1.8.0.442.6-hotspot**, select it and hit **Apply**, followed by **OK**.

* You should now see that the **Workspace default JRE** has changed to the one you just selected.

* Hit **Finish**, and then **OK**, and you are ready to roll.  The **JRE System Library** for **CS320\_Lab02** should also have been updated.

* If you do not the see **jdk-1.8.0.442.6-hotspot**, then  select **search**, and browse to the **C:/Program Files/Eclipse Adoptium** folder under **Computer**, and hit **OK**.

* Now, you can select **jdk-1.8.0.442.6-hotspot**. (**Apply**, **OK**, **Finish**, **OK**).

* You should now be able to run the lab.

Installing the JDK from Eclipse Temurin
=======================================

If you do not find the **jdk-1.8.0.442.6-hotspot** installed on your computer, you can find the instructions for installing it on the [Notes for Lab 2 Page](lab02_notes.html).

After it is installed, you can then follow the above instructions to set the **JRE System Library** to the JDK you just installed.  You can then return to the instructions above for importing the **CS320\_Lab02** projects.


Other Issues
============
There are some other issues that have been popping up with **CS320\_Lab02**.

* For some unknown reason, the **CS320\_Lab02.zip** file might be protected, and Eclipse won't let you import it.  Let me know if this continues to happen - I think this is fixed with the latest ZIP file.  You may need to log all users off the lab PC you are working on before proceeding.

* When you start Eclipse on the lab PCs, Windows might warn you about running a program that was downloaded from the Internet.  You can ignore this and move on.

* When you go to run **main()** in the **CS320\_Lab02** project, you might get a Windows Firewall warning.  You can generally hit **Cancel** and the lab will work.  if it doesn't, you might need to make changes to your specific Windows (or other) firewall settings.

Periodically, someone will come across this issue:

>	org.apache.jasper.JasperException: The absolute uri: http://java.sun.com/jsp/jstl/core cannot be resolved in either web.xml or the jar files deployed with this application

I've been looking into the issue, and came across this fairly involved post, which covers many types of different servers and scenarios.  It is not entirely helpful, but I am posting it here so that we can access it in the future: [absolute URI cannot be resolved](https://stackoverflow.com/questions/4928271/how-to-install-jstl-it-fails-with-the-absolute-uri-cannot-be-resolved-or-una)