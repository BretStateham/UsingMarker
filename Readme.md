<a name="Title" />
# Using Marker to Create Demos and Labs #
---

<a name="Overview" />
## Overview ##

This document covers how to use the Marker.exe (a markdown tool created by US DX) to create your demos.

Marker helps you create **[GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown)**.  **[Markdown](http://daringfireball.net/projects/markdown/)** is a markup language that is simpler than html, but that can be used (through a tool like Marker) to produce HTML.  **"GitHub Flavored Mardown"** adds a few features to the original [Markdown syntax](http://daringfireball.net/projects/markdown/syntax) that makes it easier to add syntax-highligted code snippets as well as a number of other items to your markdown. 

The markdown files aren't inteded for reading by a person.  The are a creation tool, not a content tool. Instead, you will use a tool like Marker to process the markdown and produce an HTML file as output.  Your readers would then read the .html file. 

While Marker helps you create **"GitHub Flavored Markdown"**, you don't need to actually use GitHub as your repository.  The marker tool produces an .HTML file that can be read anywhere.  However, if you do use GitHub as the repository for your demo files, there are some benefits because of GitHub's built-in support for markdown. 

Lastly, the Marker.exe tool is a tool that originally created by the Microsoft US Developer Platform Evangelism (DPE) team to help with creating labs and demos.  The tool was originally available in a separate GitHub repository which has since been taken off line.  I kept a .zip file with the relevant marker.exe tools in it for my personal use, and I provide that [.zip file as a resource here](./Downloads/Marker.zip).  In fact, I have [a .zip file with the entire content-tools repository contents](./Downloads/OriginalContentToolsRepository.zip) available.  I don't use the complete features available there, but there are indications of using T4 to create output, etc.  Consume it at your own risk.  

---

<a name="Prerequisites" />
## Prerequisites ##

To successfully complete this demo, it is helpful if you have a basic understanding of [Markdown](http://daringfireball.net/projects/markdown/).  The marker tool is used to create "**GitHub Flavored Markdown**" (**GFM**).  Read the following links to gain a solid understanding of **GFM**.

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

<a name="SetTheme" />

- Set the Windows Theme on your PC to match the other content creators.  This makes it significantly easier to update screenshots in the future.  

	- First, back up your current theme so you can switch back to it later. Right click on your desktop, and select **"Personalize"** from the pop-up menu.  The save the current **"Unsaved Theme"** to a name.  You can then use that saved theme name to restore your theme in the future.

		![00030-SaveTheme](images/00030-savetheme.png?raw=true "Save Theme")

	- Download the **[ResolutionsCentered.deskthemepack](./Downloads/ResolutionsCentered.deskthemepack)** file to your pc (anywhere you like), then double click on the downloaded file to apply the theme. 

---

<a name="Tasks" />
## Tasks ##

This demo is comprised of the following tasks:

- [Creating a Demo Script](#Task1)
- [Tasks, Headers, and Steps](#Task2)
- [Adding Code Snippets](#Task3) 
- [Adding Screen Shots](#Task4)

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

1. I won't cover GitHub Flavored Markdown basics here.  There is a simple and quick set of documentation available, and the links to that content was provided in the [Prerequisites](#Prerequisites) section above. [Read the documentation there](#Prerequisites) to familiarize yourself with the [markdown basics](https://help.github.com/articles/markdown-basics), and the extra features of [GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown). 


````C#
void Main() {
	int x = 1;
	int y = 2;
	int z = x + y;
	Console.WriteLine(z);
}
````

--- 

<a name="Task2" />
## Tasks, Headers, and Steps ##

As you create your demos, it is helpful to break them up into "Tasks". Tasks then can be broken down into discrete "Steps" for the reader to perform.  

Each **"Task"** should begin with a H2 tag and an anchor.  You can do that very easily by typing the text for your header, and then clicking the **"H2"** button on the toolbar.  The resulting markdown should look something like this (you can also just type two hash-marks, `##`,  at the beginning and end of your header text) :

![02005-H2ToolbarButton](images/02005-h2toolbarbutton.png?raw=true "H2 Toolbar Button")

````
<a name="my-task-header" />
## My Task Header ##
````

The actual HTML that is produced from that markdown would be something like this:

````HTML
<p><a name="my-task-header"></a></p>
<h2 id="My_Task_Header">My Task Header</h2>
````

The **name** used on the anchor tag should correspond to a Task in the task list shown near the top of the demo script.  To simplify that, I usually use use a name like Task1, Task2, Task3, etc.  That means I will modify the default anchor name like **"my-task-header"** to **"Task1"** (or an appropriate task number) like this:


````
<a name="TaskX" />
## My Task Header ##
````

Each task should start with a simple statement of the goal of the task to help the reader understand why they are following the steps in the task.  

You should then create a numbered list of "Steps" for the user to follow.  Creating the numbered list is simple.  Just start each step with **"1."** (minus the quotes).  Make sure each step is an instruction for the user to follow.  "Discussion" text should be kept in Note items related to the step.  This will help to keep each instruction simple and clear. 

YOU DO NOT NEED TO ENTER SEQUENTIAL NUMBERS.  JUST NUMBER EVERY STEP AS **1.** AND THE MARKDOWN PROCESSOR WILL CREATE THE PROPER HTML FOR YOU.

For example, the following markdown:

````
1. Do This
1. Do That
1. Do Something Else
````
Produces this HTML:

````HTML
<ol>
<li>Do This</li>
<li>Do That</li>
<li>Do Something Else</li>
</ol>
````

And it looks like this in the final HTML output (notice that the numbers used for the items are correct):

1. Do This
1. Do That
1. Do Something Else

If a task will have multiple paragraphs, sub items, or images make sure to **INDENT those subordinate items with a TAB**

For example, this markdown: 

````
1. This is a task
	
	I have a sub-paragraph for this task

1. This is another task

	> **Note:** It has a note (blockquote) as a subordinate item

1. This is a complex task that has sub list:

	- Do This
	- Then do that
	- Then do something else

1. Another task might have an image associated with it. 

	![02010-SampleImage](images/02010-sampleimage.png?raw=true "Sample Image")
````

Produces this HTML as output:

````HTML
<ol>
<li><p>This is a task</p>

<p>I have a sub-paragraph for this task</p></li>
<li><p>This is another task</p>
<blockquote>
<p><strong>Note:</strong> It has a note as a subordinate item</p>
</blockquote></li>
<li><p>This is a complex task that has sub list:</p>

<ul>
<li>Do This</li>
<li>Then do that</li>
<li>Then do something else</li>
</ul></li>
<li><p>Another task might have an image associated with it. </p>

<p><img src="images/02010-sampleimage.png?raw=true" alt="02010-SampleImage" title="Sample Image">
</p></li>
</ol>
````

And it looks like this in the final output:

1. This is a task
	
	I have a sub-paragraph for this task

1. This is another task

	> **Note:** It has a note (blockquote) as a subordinate item

1. This is a complex task that has sub list:

	- Do This
	- Then do that
	- Then do something else

1. Another task might have an image associated with it. 

	![02010-SampleImage](images/02010-sampleimage.png?raw=true "Sample Image")

1. Lastly, at the end of a task, and all it's steps, it is helpful to put a horizontal rule in the markdown so that there is a visual cue to the end of the task, and the beginning of another.  You create a horizontal rule in mardown by typeing three "hyphens" in a row:

````
---
````

Which creates the following HTML output:

````HTML
<hr>
````

And of course, looks like this in the document (see the line below this paragraph?):

--- 

Ok, so putting it all together, here is the markdown for a very simple task:

````
<a name="TaskX" />
## Simple Task ##

This task is very simple.  You'll just do three things:

1. Do this
1. Do that
1. Do the last thing

---
````

<a name="Task3" />
## Adding Code Snippets ##

It is assumed that you have already reviewed the GitHub Markdown documentation mentioned in the [Prerequisites](#Prerequisites).  GFM supports color-highlighted syntax for code blocks.  You can create a code block very simply by 

1. Copying the code from your source file

1. Pasting the code into the markdown where you want it to appear: For example, here is the initial markdown for a simple code snippet:

	````
	void Main() {
		int x = 1;
		int y = 2;
		int z = x + y;
		Console.WriteLine(z);
	}
	````

1. Selecting the pasted code, and clicking the  **"Code Snippet"** drop-down on the toolbar, and selecting the appropriate target language.

	![03010-CodeSnippetToolbar](images/03010-codesnippettoolbar.png?raw=true "Code Snippet Toolbar Button")

1. The code-snippet toolbar button will then surround the code with "fenced-code" backticks and a language indicator:

	<pre></code>````C#
	void Main() {
		int x = 1;
		int y = 2;
		int z = x + y;
		Console.WriteLine(z);
	}
	````</code></pre>

	That markup produces the following HTML:

	````HTML
	<span class="codelanguage">C#</span><pre><code class="C#"><span style="color:#0000FF">void</span> Main() {
		 <span style="color:#0000FF">int</span> x = 1;
		 <span style="color:#0000FF">int</span> y = 2;
		 <span style="color:#0000FF">int</span> z = x + y;
		 Console.WriteLine(z!!!);
	}
	</code></pre>
	````

	And finally, this is what it looks like rendered in the final page:

	````C#
	void Main() {
		int x = 1;
		int y = 2;
		int z = x + y;
		Console.WriteLine(z);
	}
	````

--- 

<a name="Task4" />
## Adding Screen Shots ##

Try to make your demo script, or lab, easy to understand by a novice.  If somebody already knew how to do what you are describing, they wouldn't need the demo script.  Imagine yourself being given this demo to perform with NO PRIOR KNOWLEDGE, and write the demo as if you were being walked through it for the very first time. 

Of course, the Prerequisites and help set the bar for how much detail is needed, but when in doubt, share.  

Screenshots are an excellent way to visually share information about the steps being performed.  The biggest downside to screenshots is that the software, website, etc. being captured often changes in future revisions.  It is helpful then to limit your screenshot to including just the pertinent parts, and to keep a consistent look and feel across them so they can be updated more easily in the future. 

In the **"Setup"** section, I outlined how to [set the theme to a consistent theme](#SetTheme).  Having a consistent theme across content developers will make it easier for one person to update screenshots created by another.

Lastly, it is helpful if your screenshots are larger than 1024x768.  The width is more restrictive than the height, so if you need to increase the height beyond 768 to show addition content, that is ok.  Images wider than 1024 can cause horizontal scrolling.  You can use a tool like [Sizer from Brainapps.net](http://www.brianapps.net/sizer/) to easily set a window size simply by right clicking on its border, and choosing your target size:

![04010-Sizer](images/04010-sizer.png?raw=true "Sizer")

Unfortunately, the tool doesn't work on all windows, including Visual Studio.  for those windows, You can rely on the "ResolutionsCentered" wallpaper included with the recommended desktop theme, and the normal Window Move and Size commands to make a window the exact size:

![04020-MoveAndSizeMenus](images/04020-moveandsizemenus.png?raw=true "Move and Size Window Menus")

[Techsmith's SnagIt](http://www.techsmith.com/snagit.html) tool is a great (but not free) utility for creating screenshots.  It allows you to create effects, outlines, add text, etc to your screen shots easily.  

Of course, you can just use the **PrtScn** button on your keyboard to capture the entire screen to the clipboard, or **Alt-PrtScn** to capture just the current window. 

Lastly, as the number of images in your demo script goes (remember, the more the merrier) They can be difficult to find, replace if needed.  You can help yourself out by giving them a sequential name.  I tend to use a format of

**ttnnn-title**

Where: 

- **tt** is the task number (01, 02, 03,...)
- **nn** is the image number (010, 020, 030, ...) leaving gaps so you can insert new images in sequence if needed.  Remember good old BASIC line numbers?
- **title** is a title WITHOUT spaces (Pascal cased)

For example, in the **second task** (02) the **third image** (030) of a **properties window** might be called something like:

**02030-PropertiesWindow**

Following is a sample walkthrough of creating a screenshot to show the reader how to get to the **Azure Documentation**:

1. In this example, we've opened the http://azure.microsoft.com website in the browser.  Then, we can use the Sizer tool (if needed) to ensure that the window is 1024x768 or smaller by right-clicking on the Window's border and selecting 1024x768:

	![04010-Sizer](images/04010-sizer.png?raw=true "Sizer")

1. Use either SnagIt, or the regular PrtScn and Alt-PrtScn keyboard buttons to capture the image.  

1. Highlight the important elements (in this case, the **Documentation** link) in the image using SnagIt's editor, the press the **Copy All** button on the **Draw** tab to copy the entire image to the clipboard.

	![04030-SnagitEditor](images/04030-snagiteditor.png?raw=true "SnagIt Editor")

1. If you don't have SnagIt, you can use PowerPoint to add shapes, etc. to highlight the important elements in the screenshot.  You can then select the image and all of the highlight elements, and copy them to the clipboard:

	![04040-PowerPoint](images/04040-powerpoint.png?raw=true "PowerPoint")

1. Copy the updated image to the clipboard, and return to marker.  Place the cursor in Marker where you want to insert the image, and hit Ctrl-V to paste the image.  If they image is within a list, make sure to indent it by pressing the **TAB** key first.  Marker actually has a recommended max width of 750 so if you image is larger than that, you will first receive a warning.  Click **"Yes"** to confirm:

	> **Note:** If you saved the image to the file system, you can also use the **"Insert Image"** button on the toolbar, but copy paste saves you having to save the file first

	![04050-Warning](images/04050-warning.png?raw=true "Warning")

1. Then you will receive a prompt asking for the **"Alt Text"** and the optional **"Title"**. Use the **ttnnn-Title** format described above for the Alt Text (NO SPACES).  The file name will be generated automatically off of that.  Then type a descriptive title, and click **"OK"**:

	![04060-PasteImage](images/04060-pasteimage.png?raw=true "Paste Image")

1. The following markup will be created for you:

````
![04070-SampleScreenShot](images/04070-samplescreenshot.png?raw=true "Sample Screen Shot")
````

1. Which in turn implies the following HTML:

```html
<p><img src="images/04070-samplescreenshot.png?raw=true" alt="04070-SampleScreenShot" title="Sample Screen Shot"></p>
```

1. And the image will appear in the rendered doc:

	![04070-SampleScreenShot](images/04070-samplescreenshot.png?raw=true "Sample Screen Shot")

1. Once you have gone through the above process a few times, but goes pretty quick.

---

<a name="Summary" />
## Summary ##

Hopefully you have a good sense of how to use the Marker tool and GitHub Flavored Markdown to create demo scripts and hands-on-labs.  Consistency is your friend.  The reader will benefit by having a consistent format for the demos and labs, and you will benefit by having a consistent content creation method.  

As needed review the topics covered in this document:

- [Prerequisites](#Prerequisites)
- [Setup](#Setup)
- [Creating a Demo Script](#Task1)
- [Tasks, Headers, and Steps](#Task2)
- [Adding Code Snippets](#Task3) 
- [Adding Screen Shots](#Task4)