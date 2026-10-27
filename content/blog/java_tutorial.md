---
date: '2026-10-26T21:04:07-04:00'
draft: false
title: 'Basic Java Developer Tutorial'
---

### Intro
This tutorial will describe how to set up a basic, functional Java Developer environment. As a good security practice, please make sure to never install software from the internet without verifying it's source. 

### Intalling your IDE 
1. For this example, we will be using Eclipse as our IDE (Integrated Development Enviroment). This is the program you will use to write and test your code. To begin, download it from [**here**](https://www.eclipse.org/downloads/packages/). Get the "Eclipse Installer" from the top of the screen. Make sure to select the appropriate version for your computer.
2. Download the Adoptium Temurin Java package [**here**](https://adoptium.net/). It should autodetect your system to provide you the correct file. On windows you will want the ".msi" version. This is an open source (free) version of the Java binary. The Java binary is what our code will interact with.
3. Now that you have both programs downloaded, lets run the eclipse installer. Navigate to your downloads folder and open the program.
4. Select "Eclipse IDE for Java Developers" (it should be the first option), then click "Install". This process may take a few minutes.
5. Another screen may pop up, asking you to verify the signers. This just means they want you to verify that the software came from a reliable source for security reasons. Hit "Select All" and then "Trust Selected".
6. Hit "Launch". This should now open our newly installed software.

### Configuring your IDE
7. Now that we have Eclipse installed, lets continue with our setup. Firstly, it will ask you what workspace you want to use. This is the location where your new projects and their code will be stored. I recommend using the default location and selecting the option to "Use this as the default and do not ask again". This will mean that every time you open eclipse it will automatically launch into this folder rather than prompting you.
8. If you've previously used eclipse, it may ask about updating your workspace. Just select "Continue".
9. After Eclipse opens, it may ask about being excluded from Windows Defender. By default, Windows Defender (the preinstlalled antivirus on all Windows Computers) will scan the files in your eclipse project for potential vulnerabilities every time you open it. This will result in slower load times and potential false positives (where your work is deleted), but it will maintian a more secure environment. I recommend selecting "Exclude Eclipse IDE", then hitting "Proceed".
10. At the "User Account Control" pop up, select "Yes". This will allow it to run the script that disables Windows Defender from scanning these files. The rest of your computer will still be protected, just not the files in the Eclipse Workspace Folder you selected earlier.

### Installing a JDK

11. Now we are going to install a JDK (Java Development Kit). This is the Adoptium file we downloaded earlier. To start, Close Eclipse.
12. Run the Adoptium file. (If you can't find the file go back to step 2).
13. Now we will go through the prompts as you would to install any other application. Select "Next". Then agree to the license agreement and select "Next" again.
14. The next screen will ask if you want to install the program for all users. I would recommend this option as it may prevent some other issues later. After you make your selection, hit "Next".
15. This menu will allow you to change how the software is installed. The default will work fine for our usecase, so select "Next".
16. Hit install, and hit "Yes" in the User Account Control Prompt.

### Further Configuration

17. Now that we have a JDK, we need to make sure it is selected in Eclipse so it knows to use it to compile and run your code. Reopen Eclipse.
18. At the top of your screen, select "Window" and then "Preferences".
19. On the left side of the screen, click the arrow next to "Java", then select "Installed JREs".
20. Make sure there is a checkmark next to "Detect available JVM Installations at startup" and at least one of the JRE files below. It should look something like this.
21. To save our changes, select "Apply" and then "Apply and Close".

### Making your First Project

22. Now that we have a development environment, we can create our first project! In the top left corner, select the "New" icon. Hovering over any of the icons in the top bar will display your name. "New" should be the furthest left icon.
23. Select "Java" then "Java Project" and hit "Next".
24. Give the project a name like "Test Project". Leave all the options as default and then hit "Finish".
25. Next we will create a class file. This is where the actual code is stored. Follow the same process as above, but select "Class" instead of "Java Project". You can give it any name, but for a single file project we typically use "main". Also select the option to create a "public static void main" method stub.
26. Congraduations! We now have our first environment ready to create some code. Add the below code into your class, between the curly braces ({}) after the public static void main method.
```
system.out.print("Hello World");
```
27. Save the program (ctrl+s), then select run (the "play arrow") in the top menu. At the bottom of the screen you should see a console window open and print 
```
Hello World
```