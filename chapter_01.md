# Chapter One: Introduction to Tools and Resources
    * Development tools and resources
    * Learning resources
    * Setting up your development environment

Developing apps for elementary OS is not much different from developing Gtk applications  for other Linux distributions, especially debian based  distributions. The major differences have to do with the few set of elementary OS specific APIs which you could (should) utilize when targeting elementary OS.

In this chapter, we will take a look at some tools and resources available to developers. Note that this guide will in some cases reference resources for you to check-out on your own. All these resources are already in existences and this guide just point you to them as I come across any during research. Beware that I do **NOT** take responsibility to ensure those resources are always available to you. However, I could make changes to this guide as situations change.

## 1.1 Development tools and resources
Tools and resources presented here are those you **MAY** need when developing (coding, documenting, building, packaging, etc.) your application.


The most obvious tool is the `vala compiler` with package name `valac` in the software repository, a copy of elementary OS installed, and a code editor or an IDE.
![Vala programming language](images/vala-description.png)

### 1.1.1 Choosing a text editor (code editor)
There are many text editors and IDEs available for vala application development, but those I have used and trusted include;

* [Scratch Text Editor](http://elementary.io): It is the default text editor pre-installed in elementary OS. It has vala code syntax highlighting and basic auto-completion by default.
![Scratch Text Editor](images/scratch.png)

* [Sublime Text](http://sublimetext.com): A fast and lightweight text editor with smart intellisense that make coding less tedious. It has vala code syntax highlighting support through the `Vala-TMBundle` package found in sublime text editor [package control](sublimetext.com).[FIX LINK]
![Sublime Text Editor](images/sublime-text.png)

* [Atom Text Editor](http://atom.io): Similar in functionality compared to sublime text but has an improved UI: feature packed with an easy-to-use point-and-click package management system (displayed with `Ctrl + ,`), well supported with a lot of packages. It has vala support through the `language-vala` and `Valhalla` packages. Downside is that it can be slow on low-end computer because it built with HTML, CSS and JavaScript.
![Atom Text Editor](images/atom-text-editor.png)

* [Gnome Builder](http://gnome.org)[FIX LINK AND SCREENSHOT): An IDE designed for developing Gnome Software with good vala support by default including code highlighting, build support good auto-completion, and devhelp integration.
![Gnome Builder IDE](images/vala-code.png)


### 1.1.2 Version Control Systems and other tools.
There are many Source code Version Control Systems available for management your application source code. Some of the most commonly used ones include;

#### Source Code Version Control Systems (DVCS/VCS)
* Launchpad: A free online service for hosting code online, collaborative development and many more.
* Bazaar: A distributed version control system of interacting with launchpad.
* Git: another source control system
* Github: A remotely hosted source code control system used in conjunction with `Git` to manage code. It offers several functionality to assist project collaboration. 

#### Other tools

##### Design tools (wireframing, mock-up, icons) 
* [Inkscape](inkscape.org): A libre vector drawing software commonly use by the elementary community for designing. It can be use for wireframing, mocking-up prototypes and icon designs.

* [Gimp](gimp.net): Another libre bitmap image editing software used for photo manipulation. While making your designs, you can use gimp to resize, crop, and apply filters on you images.

* **Sketch book and Pencil**: You may need these for the initial sketching of your designs concept and flow chart. Depending on how complex the your application will be and the number of people working on the project, you may even need to use other tools well suited for a team.

##### More tools
* [GNU debugger](gnu.org)[FIX LINK]: a tools for [debugging](wikipedia.org)[FINK LINK FOR WIKIPEDIA TOPIC] your code. There is a YouTube video on this tool [here](https://youtube.com)[FIX LINK]
* Transifex: An online resource for collaborative translation of software into other languages. 
* GTranlator or Poedit | Tools designed for translating software into different languages
* cmake: a cross-platform build system used officially in all elementary OS applications. 
* debian packaging 


### 1.1.3 Development APIs and libraries
The [official development APIs/libraries](http://elementary.io/developer) include the `Granite`, `Contractor`, `GDA` and `Soup`.
![elementary OS Official APIs](images/elementaryos-apis.png)

Several other libraries are available for use depending on the feature you want to to implement in your application (Networking, Video and Audio processing, etc.). A list of available APIs along with their documentation can be found at [valadoc.org](valadoc.org).



## 1.2 Learning resources
Learning resources are those resources available to you for learning how you can use the various development tools and resources to develop your application. Not all the resources provided here were intended for elementary OS application developers and you may have to do transfer of knowledge in some cases.  

### 1.2.1 Documentations
Since this guide assumes that you already know GTK+ and vala, those documented resources for provide here are geared towards elementary OS application development. 

* The **Developers section of elementary OS website**: This is the first resources to checkout if you want to develop for elementary OS. It has a [Getting Stated Tutorial](https://elementary.io/docs/code/getting-started), the official [Human Interface Guidelines](https://elementary.io/docs/human-interface-guidelines), and a [Reference Material](https://elementary.io/docs/code/reference). Make sure you have **REALLY** gone through all those materials before you even consider reading any other learning resource. You may need to read over and over again to make sure you familiarise yourself with elementary OS application development work-flow. 
* [Valadoc](valadoc.org): A great documentation resource for elementary OS development libraries, as well as, other libraries available for developing vala applications. It has documentation for almost all the libraries you would ever need when developing your application. Valadoc is available as an online tool but can be clone from [Github](https://github.com)[FIX LINK] and hosted locally on your computer. 
* Applications Source Code: A great way to learn something is by learning from those who know how to do it. By browsing through the source code of vala applications built for elementary OS, especially official applications, you learn a lot from their respective developers. Official application are hosted in Launchpad can be found [here](http://elementaryos.laucnhpad.net)[FIX LINK]. With Bazaar installed (`sudo apt install bzr`), you can branch/clone an application in Launchpad by entering `bzr branch lp:APP_ID` in you terminal, where `APP_ID` is the application ID. For example, entering `bzr branch lp:noise` will cone the official music application called ___Noise___.


### 1.2.2 Tutorials
#### Written tutorials
The are unofficial tutorials by third-parties;

* [eos.doodlespark.ca](http://eos.doodlespark.ca) provides a work-in-progress developer guide on the Granite framework accompanied with demo code and detailed explanation. It also has an [Icon Guide](icon names list: http://eos.doodlespark.ca/?p=icon-guide) for GTK+ icon names along with their `elementary theme` icons, grouped according to their respective categories. 
* [ Christopher Timberlake's tumblr blog](http://game64.tumblr.com) has a blog post titled ***So you want to develop for elementary OS?*** which takes you through the process of creating a demo Granite application with a `cmake` build system with detailed step by step explanation. 


#### Video tutorials
Coming soon ;)