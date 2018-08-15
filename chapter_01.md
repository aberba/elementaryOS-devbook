# Chapter Two: Introduction to Tools and Resources

```
* Learning resources
* Development tools
* Setting up your development environment
```

Developing apps for elementary OS is similar to developing GTK+ applications for other Linux distributions. The major differences are the tools and resources including some elementary OS specific APIs which you can utilize when developing for elementary OS. This not only boost developer productivity but also provides a better developer experience.

In this chapter, we will take a look at some tools and resources available to developers. Note that I will in some cases reference resources for you to check them out.

## Learning Resources
Since this book assumes that you already know (at least basic) GTK+ and Vala, those learning resources provided here are geared towards elementary OS application development.

### The developers page of the elementary OS website
This developers page provides some official guides from the elementary OS core developers. It has a [Getting Started](https://elementary.io/docs/code/getting-started) tutorial, [Human Interface Guidelines](https://elementary.io/docs/human-interface-guidelines), and a [Reference Material](https://elementary.io/docs/code/reference). These resources will help familiarize yourself with the app development workflow including recommended design practices and code style guides.s

### Valadoc
[Valadoc](https://valadoc.org) is a great documentation resource for elementary OS development libraries, as well as, other libraries available for developing Vala applications. It has documentation for almost all the libraries you would ever need when developing your application.

### Application Source Codes
A great way to learn something is by learning from those who already know how to do it. By browsing through the source code of Vala applications built for elementary OS, especially official applications, you learn a lot from their respective developers. Official applications are hosted in the elementary GitHub repository at https://github.com/elementary. Source code of third-party applications published in the App Center may also be a great learning resource.

## Development Tools
The following tools presented here are those you *need* when developing (planning, designing, coding, etc.) your application. These included elementary OS, the Vala compiler and a text editor or an Integrated Development Environment (IDE).

### Choosing a text editor or an IDE
There are many text editors and IDEs available for Vala application development including  [Atom](http://atom.io), [Scratch Text Editor](http://elementary.io), [Visual Studio Code]() and [Gnome Builder](https://wiki.gnome.org/Apps/Builder). However, I will use the default IDE which comes preinstalled in elementary OS called **Code**. Code comes with good support for Vala programming language out of the box, including syntax highlighting, auto-completion, find and replace, symbol list**FIX and multi-line commenting.

![Code, the default text editor preinstalled on elementary OS](images/scratch.png):

### Source code management and other tools.

[GitHub](https://github.com) is web-based Git repository hosting service and the officially supported source code management platform for elementary OS application development. It offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features. Features offered by GitHub helps in managing issues like bugs, feature request from users, and submitting an application to the elementary OS app center.

> **Git** is a source code management system which you can use to manage your code during development and other version control tasks. GitHub and Git are discussed into details in Chapter 4 of this book.

Below are some other tools you may when developing your application:

#### Design tools (wireframing, mockups, icons)

* [Inkscape](inkscape.org): A libre vector drawing software commonly use by the elementary community for designing. It can be use for wireframing, mocking-ups and icon designs. The icons of all official elementary OS applications are designed in Inkscape. 

![Inkscape](images/inkscape.png)

* **Pencil and Paper**: You may need a pencil and paper for the initial sketching of your design concepts and flow chart. Depending on how complex the your application will be and the number of people working on the project, you may even need to use other advanced tools for collaboration.

### Development libraries
The [official development libraries](http://elementary.io/developer) include the `Granite`, `Contractor`, `GDA` and `Soup`. ![elementary OS Official APIs](images/elementaryos-apis.png).

Several other libraries are available for use depending on the feature you want to to implement in your application (Networking, Video and Audio processing, etc.). A list of available APIs along with their documentation can be found at [valadoc.org](https://valadoc.org)

## Setting Up Your Development Environment
This section will help you set up the necessary tools and resources to get your computer ready for development. The elementary OS project has set up a [Getting Stated Tutorial](https://elementary.io/docs/code/getting-started) tutorial which includes a section for setting up your development environment. By following that guide, you should be able to install all dependencies such as cmake, Granite, Bazaar, GTK+, etc, as well as, create a Launchpad account. These are the basic setup required for development.

### Using a third-party text editor

The default text editor that is pre-installed in elementary OS, Scratch, is good for basic code editing but I recommend _Sublime_ or _Atom_ text editor for better coding experience. Below is how you can set up either one those text editors.

#### Installing and configuring Sublime text editor

Download and install Sublime Text Editor (Version 3) from <http://sublimetext.com>. Since Sublime does not come with vala syntax highlighting by default, you may have to install the `Vala-TMBundle` package. You can install this package by downloading it and installing manually or using the Sublime Package Control within the text editor. Using the Sublime Package Control approach is what I recommend to be able to make future package updates and installations right from Sublime.

##### Configuring and installing from the Package Control

To install using the package manager make sure you have Internet connection since the packages will be fetched from the package control from a remote server.

* Go to <http://pakagelink.com>, copy the piece of code from the ....[FIX THIS],
* Open Sublime on your computer and paste the code in the Console entry box displayed by pressing `Ctrl + [back-tick]` on your keyboard or `View > Show Console` from the menu.
* Press `Enter` and wait for the script to configure the package control. After successful configuration, Sublime is now be ready to install the `Vala-TMBundle` package as well as any other package in the future right from the text editor.
* You can now display the Package Control by pressing `Ctrl + Shift + P` or `Preferences > Package Control`. Using the Up or Down key on your keyboard, navigate to `Install Package` and press Enter. Wait for Package Control to fetch the list of packages from the remote server (this may take some few seconds depending on your Internet connection speed). When all the packages are fetched, you will see the list of packages in the Package Control dialog displayed at the upper middle corner in the Sublime.
* Search for `Vala-TMBundle` using the search entry within the dialog, navigate to the Vala-TMBundle package, press Enter to install it. You are now ready to start coding with sublime :)

##### Installing packages manually in Sublime

To install `Vala-TMBundle` manually, go to the Github repository of the package at <https://github.com>[FIX THIS LINK] and download the package source by clicking on green `Clone` button and then the `Download Package zip`[FIX THIS] link. Open Sublime and click on `Preferences > Browse Packages` from the main menu. This will open the location where Sublime packages are installed in your file manager. Unzip the `Vala-TMBundle` archive and copy the unzipped copy (the whole folder) into `User` directory within the package install location. Restart sublime and you are ready to go :)

#### Installing and configuring Atom text editor

Installing packages in Atom Text Editors is much easy and straight forward compared to Sublime. Whilst making sure you have Internet connection;

* Download and install Atom form their website at <https://atom.io>
* Open Atom and display the package manager clicking on `Packages > Settings View > Install Packages/Themes` from the main menu.
* Wait for Atom to fetch for the list for available packages and search for `language-vala` and `Valhalla` and install both. You may also want to install the `terminal-plus` package to get a terminal within Atom. You are now ready to start coding with Atom.

### Using valadoc documentation offline

Using valadoc.org requires that you have persistent Internet connection. However, there are two ways you can use the valadoc offline: (1) running valadoc on a local server on your computer or (2) downloading compressed HTML documentation files for each individual library you would like to use.

To use run a local server for valadoc visit their [Github repository](https://github.com/flobrosch/valadoc-org) where they have instructions on how to do that. To download compressed html documentation files, visit valadoc.org and scroll down to the your library of choice and click on the `Download documentation`[FIX ME] to download a compressed copy of the documentation of that library. You can now extract the contents of the downloaded file which contains the HTML documentation files.

> ### Tip to convert any web page to PDF

> Saving web pages as HTML files could make your directories cluttered. You could instead save any web page as PDF right from you browser by pressing `Ctrl + P` as if you are printing the page and then click on `Print to File` from the print dialog. Choose where you want to save the file as PDF and click print to save.
