<a name="Title" />
# Using Marker to create Demos #
---

<a name="Overview" />
## Overview ##

This document covers how to use the Marker.exe (a markdown tool created by US DX) to create your demos.

---

<a name="Prerequisites" />
## Prerequisites ##

To successfully complete this demo, it is helpful if you have a basic understanding of [Markdown](http://daringfireball.net/projects/markdown/).  The marker tool is used to create "**GitHub Flavored Markdown**" (gfm).  Read the following links to gain a solid understanding of gfm.

- [GitHub Markdown Basics](https://help.github.com/articles/markdown-basics)
- [GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown)
- [GitHub Mastering Markdown Guide](https://guides.github.com/features/mastering-markdown/)


---

<a name="Setup" />
## Setup##

Before starting this demo, you must:

- Download the **[marker.zip](./Downloads/Marker.zip)** file and extract it to a folder on your computer. 
	- Run the **"Marker.exe"** tool to launch Marker.  You may want to place a shortcut to the .exe file on your start screen, taskbar or desktop.
	- The first time you run **"Marker.exe"** it may prompt you to associate the **&lowast;.md** file extenion with Marker.  Allow the association. If you need to reset the association again, you can do it from the Marker's menu bar, and the **"Tools"** | 

	![00010-AssociateMdExtension](images/00010-associatemdextension.png?raw=true "Associate .md Extension")

- Download and install the **[Sizer](http://www.brianapps.net/sizer/)** utility.  Sizer makes it easy to resize a window to a specific size.  It is recommended that you use a reference dimension of 1024x768 for your screen shots.  Sizer helps you set windows specifically to that size. 

	![00020-Sizer](images/00020-sizer.png?raw=true "Sizer")

- If you have access to **[SnagIt from Techsmith](http://www.techsmith.com/snagit.html)**, I highly recommend using that as a screen shot utility.  It makes it simple to create and edit screenshots for use in your demos.

- Set the Windows Theme on your PC to match the other content creators.  This makes it significantly easier to update screenshots in the future.  

	- First, back up your current theme so you can switch back to it later. Right click on your desktop, and select **"Personalize"** from the pop-up menu.  The save the current **"Unsaved Theme"** to a name.  You can then use that saved theme name to restore your theme in the future.

		![00030-SaveTheme](images/00030-savetheme.png?raw=true "Save Theme")

	- Download the **[ResolutionsCentered.deskthemepack](./Downloads/ResolutionsCentered.deskthemepack)** file to your pc (anywhere you like), then double click on the downloaded file to apply the theme. 

---

<a name="Tasks" />
## Tasks ##

This demo is comprised of the following tasks:

- [Creating a Demo Script](#Task1)
- [Adding Code](#Task2) 
- [Adding Screen Shots](#Task3)

--- 

<a name="Task1" />
## Creating a Demo Script ##

In this task, you'll create a basic demo script using the template.  If you are working in a repository that has already been setup, then you may not need to do this, the initial structure may already be in place.  But if this is a new repository, and you are creating the structure, these steps will get you started. 

1. Download the [Demo.zip](./Downloads/Demo.zip) file to a folder on your PC.  

1. Right-click on the downloaded **"Demo.zip"** file, and select **"Properties"** from the pop-up menu:

	![01010-Properties](images/01010-properties.png?raw=true "Properties Menu Item")

1. In the **"Demo.zip Properties"** window, click the **"Unblock"** button.  Then click the **"OK"** button to close the window.

	> **Note:** This will keep Windows from prompting you with security concerns when you use extracted files.

	![01020-DemoZipProperties](images/01020-demozipproperties.png?raw=true "Demo.zip Properties")

1. Right-click on the **"Demo.zip"** again, this time select **"Extract All"** from the pop-up menu, then in the **"Extract Compressed (Zipped) Folders"** window, browse to, or type the target directory for the extraction, and click **"Extract"** 

	![01030-ExtractZip](images/01030-extractzip.png?raw=true "Extract Demo.zip")

1. You should now see the contents of the .zip file:

	![01040-DemoZipContents](images/01040-demozipcontents.png?raw=true "Demo.zip Contents")

	- **Assets Folder** - This is where you will place any assets or resources that are needed during the demo.  Things like Logo Images, completed code files, data files, etc.. Please try to keep a logical structure to the contents.  

	- **Begin Folder** - This is where you will place any starter projects and solutions.  If the demo is long, it is helpful to have starting projects for various milestones throughout the project. 

	- **End Folder** - This is where you will place any completed projects.  Again if the demo is long, it is helpful to have completed versions of the project at various milestones. Honestly, these are often the same as the **"Begin"** milestone projects.  The completed project from one step, is the beginning project for the next.  Regardless, you should have at least a single FINAL completed version of the projects.  

	- **Images Folder** - Contains the images that you paste into the demo script in Marker. Marker uses this folder by default when it creates images on your behalf. 

	- **Readme.md** - This is the actual demo script.  Naming it Readme.md rather than Demo.md or anything else makes it appear by default in the GitHub.com website view of the Demo folder.  


````C#
void Main() {
	int x = 1;
	int y = 2;
	int z = x + y;
	Console.WriteLine(z);
}
````
1. Do _That_ - I try to keep my screen shots to no bigger than 1024x768.  That is still bigger than what the Marker tool recommends, but it has worked well for me previously.  

	![01010demoimage](images/01010demoimage.png?raw=true "Demo Image")

1. Do ***The Other Thing***

	> **Note:** This is a note

--- 

<a name="Task2" />
## Task 2 ##


In this task we'll......

1. One

1. Two 

1. Three

--- 

<a name="Task3" />
## Task 3 ##


In this task we'll......

1. One

1. Two

1. Three

---

<a name="Summary" />
## Summary ##

In this demo we completed the following tasks:

- [Task 1](#Task1)
- [Task 2](#Task2) 
- [Task 3](#Task3)

