---
layout:     post
title:      Setting up Flutter development environment for Windows
subtitle:   Flutter Madness!!
date:       2021-09-06 12:00:00
author:     "GDSC | Shrihari S"
header-img: "img/inpost/Flutter-logo.png"
catalog: true
tags:
    - Setup Flutter
    - Flutter in windows
---


### Setting up Flutter development environment for Windows

> As a developer, I’ve always wanted to try out flutter for a long time.
> When I started with Flutter, Setting it up ate a lot of my time, I had
> to go through various tutorials, and articles to set up the
> development environment. I’m writing this blog as I don’t want my
> fellow developers to face the errors that I had to, during
> the process.

![](https://cdn-images-1.medium.com/max/800/1*qfQKFPgYV997X2tSEY2EVA.png)

#### System Requirements:

*To install and run Flutter, your development environment must meet
these minimum requirements:*

-   **Operating Systems**: Windows 7 SP1 or later (64-bit), x86–64
    based.
-   **Disk Space**: 1.64 GB (does not include disk space for IDE/tools).
-   **Tools**: Flutter depends on these tools being available in your
    environment.
-   [Windows PowerShell
    5.0](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-windows-powershell)
    or newer (this is pre-installed with Windows 10)
-   [Git for Windows](https://git-scm.com/download/win) 2. x, with the
    **Use Git from the Windows Command Prompt** option.
-   If Git for Windows is already installed, make sure you can run
    `git` commands from the command
    prompt or PowerShell.

* * * * *

### Things to Download/Install:

The following are what you are going to download/install during the
process:

-   **Flutter** SDK

> SDK — Software Development Kit

-   **Andriod Studio**
-   **Java SE** Development Kit
-   **Git**for windows
-   **VS Code** (Visual Studio Code)

> Let’s get started, shall we?

#### Flutter SDK(Software Development Kit):

![](https://cdn-images-1.medium.com/max/800/1*8Scn11YFwAufMziA4C5cuw.png)

A clip from
[https://flutter.dev/docs/get-started/install/windows](https://flutter.dev/docs/get-started/install/windows)

You can download the latest stable version of Flutter SDK from the
[**Official Flutter installation
documentation**](https://flutter.dev/docs/get-started/install/windows).
The current stable version for windows is 2.2.3-stable, which might not
be the same when you’re reading this blog. Download the latest version
that is available at that time.

-   Extract Flutter SDK from .zip
-   Create a folder in your C: Drive `C:\src` and paste the extracted flutter SDK.

![](https://cdn-images-1.medium.com/max/800/1*qCE5yeyMlyDeepnDFMxKtQ.png)

Flutter SDK in C Drive

-   Now go inside the flutter folder and then into the bin.
-   Copy the path of the bin.

![](https://cdn-images-1.medium.com/max/800/1*ffRspqEV6-GvMAwU35H3Ag.png)

-   Open your windows search and type `env`.

![](https://cdn-images-1.medium.com/max/800/1*fgb_9tlEY2B508_8B5XzNw.png)

-   Now open the “Edit environment variables for your account”.

![](https://cdn-images-1.medium.com/max/800/1*57jfXI6YITOhE1UwQWieQA.png)

-   Double click `path`

![](https://cdn-images-1.medium.com/max/800/1*MnMskKfaKdoScCrPlROG2g.png)

-   Click `New`and paste the path of the
    `flutter\bin` and click “Ok”.
-   Now, open your cmd (or any terminal window) and type this.

```
where flutter dart
```

![](https://cdn-images-1.medium.com/max/800/1*yrC9vZvI3mMVrkyBxjQjDA.png)

If you get the location of flutter and dart files, you have successfully
installed flutter SDK and set its path 🥳.

* * * * *

#### **Java SE** Development Kit:

> If you already have JDK installed on your pc, make sure that you’ve
> set it to the path “JAVA\_HOME”.

**Now, let's set up Java SE :**

-   Download “Java SE 8” from [JDK SE 8
    DOWNLOAD](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html).
-   Under “Java SE Development Kit 8u301”, you’ll see this

![](https://cdn-images-1.medium.com/max/800/1*ncXhO8im-U9011zY5hJihg.png)

[https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)

-   Download and Install x64/x86 w.r.t. your PC’s specification.
-   After installing, navigate to `\bin`
    of JDK, in my case:

```
C:\Program Files\Java\jdk1.8.0_301\bin
```

-   Copy the path, open “Edit environment variables for your account”.
-   Create a new variable `JAVA_HOME`.

![](https://cdn-images-1.medium.com/max/800/1*WN-g6DU3JSTJ14exvRIuaQ.png)

JAVA\_HOME Environment Variable

You’re done setting up the JDK. 🥳

* * * * *

#### Andriod Studio:

> We’re downloading andriod studio to set up the andriod emulator.

-   Download Andriod Studio from [ANDRIOD
    STUDIO](https://developer.android.com/studio).
-   Install it.
-   Now, open your CMD/Terminal, and run the command:

```
flutter doctor
```

-   See if `flutter doctor` recognized
    android studio

![](https://cdn-images-1.medium.com/max/800/1*UlFt_y2Mo-exlicmuD-VxA.png)

> You might not get Green Ticks on everything, check only andriod studio
> as of now.

-   If Flutter cannot locate it, run
    `flutter config --android-studio-dir <directory>`{.markup--code
    .markup--li-code} to set the directory that Android Studio is
    installed to.
-   Open Andriod Studio

![](https://cdn-images-1.medium.com/max/800/1*XFGOQTXTfy8L-ijJcZmFBw.png)

Andriod Studio

> If you wish to develop flutter apps in Andriod Studio itself,

> - Go to plugins, search for “Dart” and “Flutter”.

> - Download them, and restart andriod studio. Now you’ll be able to see
> a “Create New Flutter Project” on the dashboard.

-   Select `More Actions`.

![](https://cdn-images-1.medium.com/max/800/1*xO9kog7CVnCtgJ6nuViXCw.png)

Andriod Studio

-   Choose `AVD Manager`.

![](https://cdn-images-1.medium.com/max/800/1*wsgdvzS6GWqArAYsN5VYww.png)

AVD Manager — Andriod Studio

-   Click `+ Create Virtual Device…`.

![](https://cdn-images-1.medium.com/max/800/1*rV_wNMSp-bmcBTSlez641Q.png)

Create Virtual Device — AVD Manager — Andriod Studio

-   Choose an Andriod device of your liking and click Next.

![](https://cdn-images-1.medium.com/max/800/1*WVw3y4jiA62EJqslLlWuLg.png)

Create Virtual Device — AVD Manager — Andriod Studio

-   Download the Andriod version you want by clicking
    `Download` (blue), under
    `Release Name` .
-   Once, it’s downloaded, click Next.

![](https://cdn-images-1.medium.com/max/800/1*D4WAPz6sPY9h_soO8jRsXw.png)

Create Virtual Device — AVD Manager — Andriod Studio

-   Now, Finish.

🍻Cheers to you, you’re almost done!. 🥳


#### Visual Studio Code:

> Say Hello to my favorite IDE!

-   Download VS Code from [VS CODE
    DOWNLOAD](https://code.visualstudio.com/download).
-   Install and open VS Code.
-   Open Extensions.

![](https://cdn-images-1.medium.com/max/800/1*t6fkkTxoJPHxnNq41L8WPw.png)

Extensions — VS Code

-   Search for`Flutter` in the
    extensions, and install this:

![](https://cdn-images-1.medium.com/max/800/1*HDeja0a7oWjRVrViwsL3YQ.png)

Flutter Extension — VS Code


> Yayyy, Everything’s done. Now, it’s time for Flutter Doctor’s
> Checkup!.

-   Open CMD/Terminal, and run

```
flutter doctor
```

-   You might still have one box unchecked.

![](https://cdn-images-1.medium.com/max/800/1*-UKIvpxPpoiPJOjggA8HHg.png)

Flutter Doctor

-   Run this command on your terminal,

```
flutter doctor --andriod-licenses
```

-   Now, run `flutter doctor` again.

![](https://cdn-images-1.medium.com/max/800/1*SFXo91di06Fzy9L-Nr8dQg.png)

Flutter Doctor

> Yippieee, now you’re all set for developing Flutter Applications!.

A 👏 to the blog would make me Happy😊 and encourage me to write more
blogs like this!.

If you get any Doubts/Errors🤔 during the setup💻, the comment section is
all yours!. I’ll reply as soon as possible.

If you have any suggestions for my next post, feel free to drop them in
the comments section.

Interested in connecting with me? I’ve shared my LinkedIn profile below.

[**Srihari S - Technical Team Member - DSC SRMIST Ramapuram Campus |
LinkedIn**\
*View Srihari S' profile on LinkedIn, the world's largest professional
community. Srihari has 1 job listed on
their…*www.linkedin.com](https://www.linkedin.com/in/srihari-sundaramurugan/ "https://www.linkedin.com/in/srihari-sundaramurugan/")[](https://www.linkedin.com/in/srihari-sundaramurugan/)
