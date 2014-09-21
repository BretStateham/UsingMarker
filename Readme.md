<a name="Title" />
# Using Marker to Create Demos and Labs #
---

<a name="Overview" />
## Overview ##

This document covers how to use the Marker.exe (a markdown tool created by US DX) to create your demos.

Marker helps you create **[GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown)**.  **[Markdown](http://daringfireball.net/projects/markdown/)** is a markup language that is simpler than html, but that can be used (through a tool like Marker) to produce HTML.  **"GitHub Flavored Mardown"** adds a few features to the original [Markdown syntax](http://daringfireball.net/projects/markdown/syntax) that makes it easier to add syntax-highligted code snippets as well as a number of other items to your markdown. 

The markdown files aren't inteded for reading by a person.  The are a creation tool, not a content tool. Instead, you will use a tool like Marker to process the markdown and produce an HTML file as output.  Your readers would then read the .html file. 

While Marker helps you create **"GitHub Flavored Markdown"**, you don't need to actually use GitHub as your repository.  The marker tool produces an .HTML file that can be read anywhere.  However, if you do use GitHub as the repository for your demo files, there are some benefits because of GitHub's built-in support for markdown. 

Lastly, the Marker.exe tool is a tool that originally created by the Microsoft US Developer Platform Evangelism (DPE) team to help with creating labs and demos.  The tool was originally available in a separate GitHub repository which has since been taken off line.  I kept a .zip file with the relevant marker.exe tools in it for my personal use, and I provide that .zip file as a resource [here](./Downloads/Marker.zip).  


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

	![01050-ReadmeMdDisplay](images/01050-readmemddisplay.png?raw=true "Readme.md Displays be Default in GitHub")

1. Now open the Readme.md file in Marker.exe.  If you successfully created the file associations as described in the **"[Setup](#Setup)"** section, you should be able to just right click on the file.  If not, just run Marker.exe from wherever you extracted it, and use the **"File"** | **"Open"** menu item to open the **"Readme.md"** file that you extracted into your demo folder.

	***Open by File Association:***

	![01060-MarkerAssociationIcon](images/01060-markerassociationicon.png?raw=true "Marker File Association Icon")

	***Open from Marker menu:***

	![01070-OpeningReadMe](images/01070-openingreadme.png?raw=true "File Open Readme.md")

1. Regardless of how you open it, you should now see the default Readme.md file in Marker.

	![01080-ReadMeInMarker](images/01080-readmeinmarker.png?raw=true "Readme.md in Marker")

1. You should notice that there are two "columns" in the main Marker interface.  The left hand column is where you edit your Markdown.  The right-hand column is a live preview of the HTML web page that will be created based on your markdown. 

	![01090-MarkerColumns](images/01090-markercolumns.png?raw=true "Marker Columns")

1. Finally, you should see sample content for a demo.  You can simply replace the demo text with text that is appropriate for your demo, and of course add to it what is needed. Take some time to play around with the various toolbar and menu items to discover what they help you do:

	![01100-MarkerToolbar](images/01100-markertoolbar.png?raw=true "Marker Toolbar")

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

