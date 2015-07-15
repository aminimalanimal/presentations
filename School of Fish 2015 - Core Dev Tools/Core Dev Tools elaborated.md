# Core Dev Tools and Process

2015 07 15 morning

<!-- MarkdownTOC depth=4 -->

- Intro
- Sublime Text
	- Interface Basics
		- Opening Your Project
		- Navigating
		- Columns
		- Word Wrap
	- Working with Multiple Cursors
		- Copy/Pasta
	- Customizing Your Sublime Workflow
		- Preferences
		- Command Palette
- Documentation
	- Commenting in Sublime
	- Markdown
		- Markdown Editing
		- Syntax
		- Markdown Preview
		- Markdown TOC
		- Mou
- SourceTree
	- Introduction to the Interface
	- Basic Tasks
		- Cloning a Repo (or adding an existing one)
		- Adding a Remote
		- Committing/Pulling/Pushing
		- Branching
		- Merging
	- Advanced Tasks
		- Git Log
		- Git Blame
		- Interactive Rebasing
		- Rebasing (ONLY ON YOUR LOCAL BRANCH)

<!-- /MarkdownTOC -->


## Intro

Hi guys. Welcome to Core Dev Tools. My name is James Curd. I'm a presentation layer engineer. I've been here for about two years, working primarily on the {{client}} project. Today we're going to be talking about Sublime Text 3, SourceTree, and Markdown. Two of those are programs, Markdown is a language for documenting your work, and they all fit together rather well—at least in my daily workflow.

Now you're by no means obligated to use these tools. The majority of the {{client}} team does use Sublime Text, but about half uses SourceTree. SourceTree doesn't do anything that Git doesn't do, but presents it to you in a visual manner that I find it easier to work with.

However even if you choose not to use these tools it's likely that other tools will have a equivalent functionality. So if you see something today that you think is helpful I suggest you find out if you can use it in your code editor of choice.

With Sublime Text, you'll learn to rapidly find what we're looking for in large projects—and who wrote it, write code faster and cleaner, reduce errors with syntax highlighting, linters, and git integration.

With SourceTree, you'll learn to perform most Git operations free of command line, allowing you to easily overview code changes and prepare clean commits you can feel confident in.

With Markdown, you'll learn to document and write about code—allowing you to communicate gracefully in GitHub, StackOverflow, README files/etc.

## Sublime Text

So let's start with sublime text. We made a JIRA ticket for you to download this before this class. Has everybody completed that? Cool.

### Interface Basics

#### Opening Your Project

Cool. Let's go over the basics of the interface. So to open your project sublime text, you can do want to three things. You can either drag the folder of the project into the icon of sublime text in the dock. You can open sublime text, go to file menu bar, and click up and then navigate to the folder and click okay. Or you can launch it from the command line, which requires a little bit of behind-the-scenes configuration that we aren't going to get into now, but here's a link if you want to do that: http://olivierlacan.com/posts/launch-sublime-text-3-from-the-command-line/

{{Display Link}}

#### Navigating

Okay, so navigating.

##### Side Bar

On the left hand side of the screen you'll see some sublime text' sidebar. You can show and hide it with command plus K and then B.

{{Do this with Onscreen key command thing on}}

Clicking on an item in the side bar will open it. Right clicking on items sidebar will have more options. You can increase the number of options that you get by installing an extra package. We'll get to that later.

##### Goto Anything

One of my most used commands and sublime text is goto anything. Press command plus P and we'll see a little prompt comes up. Now we can start typing whatever we want to try to get to the file that we're looking for. Now this prompt is really cool because it's not just about typing the name of the file—it will also grab things out of the file's path, and it utilizes fuzzy search, which means you can actually abbreviate things in that as well.

{{Demonstrate}}

I find that using goto anything is far faster than looking at the sidebar, and so most of the time I turn my sidebar off entirely to have the extra screen space.

Also within go to anything, we can type ":" the then a line number to jump immediately to that line in the file that you're in.

##### Find

Now got anything is cool, but we also need the ability to Find throughout project.

Command plus shift plus F we'll let you search through whatever specified folder you want. Typically I remove everything in the "Where" category, and use some very basic regex instead. With nothing in that ware category it will by default only search through folders that you've already included in the current workspace. So if you want to search for something that's in one of your JavaScript files, we can type *.JS, then enter whatever you want into the find field and hit Find.

{{Demonstrate}}

You'll see that it brings us to screen of results. Now There're couple ways that we can ask for sublime text display this, and that's what this little use buffer icon does. If uses buffer isn't checked you get the results below your open files if it is checked you get it in one of the windows that you would naturally be looking in.

Now we can double-click the name of the file in order to jump straight into it, you can double-click one of the lines that I found a result to jump straight to that line in that file.

{{Demonstrate}}

Let's go who will icons left for a quick. Very left we have regular expressions. This can be incredibly powerful I personally find it difficult to come up with regular expressions on-the-fly, but if you're already well-versed in them, this can help substantially.

Link to regexr:
http://www.regexr.com

Her second icon is case sensitivity pretty obvious third is whole words that will match things only if what you have typed is the entire word rather than being a part of the word. For example if I'm looking for usage of links within CSS files, searching for A by itself wouldn't be very helpful, because usually able return results that are within properties, and not just elements.

{{Demonstrate}}

The Show Context icon will provide you with Lines on other side of the matching result. And we've already gone over the use buffer icon.

Side note: When you Replace All from this view, Sublime Text will open every file that that gets replaced in and require you to save them. You can do this individually or you can find save all from the file menu.

#### Columns

Cool. Moving on we have the ability to change the amount of columns that we have on screen.

- `command` + `option` + `1`/`2`/`3`/`4`

{{Demonstrate}}

#### Word Wrap

When you're working with multiple columns, code is likely to be long enough to require horizontal scrolling. Alternatively you can turn on word wrap from the view menu.

___

### Working with Multiple Cursors

So This is one of my favorite things about sublime text and I understand that other code editors have picked up on this. (Atom, Coda. Even Codepen can do it.) Let's get into working with multiple cursors.

Now, there are several ways to get multiple cursors on the page.

You can command plus click in order to place a second cursor down wherever you clicked.

{{Demo}}

You can use command plus D while you're highlighted on a word to select the next instance of that. This is the one that I usually use.

{{Demo}}

Command plus control plus G will select all instances of that word throughout the file.

{{Demo}}

Using control while clicking and dragging and this actually allows you to select an entire column.

**{{Create Demo for this that actually makes sense.}}**

We can use `control` + `option` + `^` and `v` arrows to select the line above or below.

{{Demo}}

Your screens probably just did something really weird if you were following along. We actually have to change a setting in OS X in order to free up those commands.

I find that particular key combination to be useful so we're going to do just that.

Keyboard > Shortcuts > Application Windows

So you might be thinking to yourself—what is the point? Why would I want to work with multiple cursors? I actually use this all the time I don't even like writing editors anymore because this is the killer feature to me.

There are a couple of systemwide commands that really increase the power of multiple cursors.

At least, they're _nearly_ systemwide. I found that attempting to use these commands within commandline and Adobe products tends to produce unexpected results.

Hold down option and you click left and right keys you can skip a word at a time. Now by default, sublime text is going to see hyphens as a word separator. We can actually change that, and we'll get to that in a moment.

{{Demo}}

OS X also allows you to navigate with command plus left and right arrows, goodness will jump into the end of the line and if you hit it again it will take you to the end of the paragraph.

{{Demo}}

#### Copy/Pasta

The sublime text, you can copy an entire line just by being on the line. Simply hit command plus C—your usual copy command, and now you've got the entire line on the clipboard.

When you're using multiple cursors and you copy the entire line in this way, when you paste your going to end up with multiple instances of those lines, and that's probably not what you intend to do.

{{Demo}}

So if we use command plus left arrow, we can jump to the beginning of our line, hold shift, and use command plus right arrow twice in order to select the entire thing. Now when we paste, each individual cursor will remember its own part of the clipboard.

{{Demo this with `for` and `id` on inputs, copying the `for`, and pasting it into `id`}}

Sublime text also has a feature that tries to be a little bit smarter about how it pastes.

You might notice that if you grab a code block that is indented to far in one direction and then paste it under another code blocks that has a different indentation, that you're going to have to adjust your indentation.

{{Demo with javascript blocks}}

Using command plus shift plus V will attempt to get the indentation correct automatically rather than pasting the lines verbatim.

Of course we'll still probably have to shift our indentation a little bit. We can use command plus [ or ] to shift line we're on left to right. The bottom right-hand corner of sublime text you'll see a thing that says tab size. Clicking on this allows you to adjust preferences for the file you are in. Sublime tries to be predictive about this, and you can also explicitly set this within your user preferences.

### Customizing Your Sublime Workflow

#### Preferences

Alright let's get back to customizing our preferences.

Under the sublime text menu, click preferences, and then we can see default preferences and user preferences. The preference files or just JSON, and at least initially the User preferences file will be pretty empty.

When you customize preferences always customize the user preferences file. If you make changes to the default preferences file, when sublime text updates those changes will be lost. The default file is a good reference for what you can overwrite.

Earlier in mentions changing how word separator's work. Essentially I taken the key value pairing from the default preferences copied it into the user preferences, and removed the hyphen.

We can also set what we want our standard tab size to be whether or not we want to translate tab spaces and whether or not we want to supply them to attempt to detect the indentation of the file by default.

You can also customize the look and feel of sublime from here. We have fun size color scheme the ability to highlight the line here on change boldness of folders on the sidebar I like the modified tabs that you have and even provided and nifty vertical column to help you understand what level you're indented in.

One of the most important things you are going to do here though, is set which folders and file types you want to exclude from seeing in sublime text. The folder exclude patterns are especially important when you're working in a project that has a build process that's going to output code that's different from the code that you're working in. By excluding the build or distribution folder here you can prevent yourself from accidentally altering output files, which can be a fairly common and confusing mistake. Make an edit, look at the browser, don't understand why you don't see changes... A lot of times that's because you're working in the wrong file. So cut the clutter here kick out all of your node modules, vendor scripts, your sass cache, your bower components, and your distribution stuff and that way you'll only see what you need to actually be modifying.

#### Command Palette

###### Installing Package Control

https://packagecontrol.io/installation

Simple installation. Run the python command and restart and we're done.

Alright, now we're going to jump into the command palette. Hit command plus shift plus P to open the palette. From here you have access to generally anything sublime text can do and as was the case with go to anything we have the ability to fuzzy search.

Most of the power from this is going to come from plug-ins that you install. We have to install package control manually, but after that we'll be able to search for and install uninstall and alter our installed plug-ins with the ease of the command palette.

**{{Step through installing this}}**

Okay does everybody have it installed?

###### Syntax Highlighters

If you ever start using a preprocessor language it may not have syntax highlighting and supplying by default we can have these highlighters simply by using package control and looking for one. Let's say we have decided to use Jade. We can use command plus shift plus P to open up the command palette, then start typing "install package". Cool it's installing and we can see the bottom there that it... just finished.

Let's open up a new file with command plus n, then open up our command palette again and start typing SYN Jade. Cool. Now if you have a filed ends in `.jade`, it should automatically pick up that you should be using Jade syntax for the jade file. If for any reason it doesn't, you can go to view syntax open all with current extension as... And choose the syntax that you want to associate with the file type.

###### Linters

Okay syntax highlighters are helpful but let's get into linting. Linters point out mistakes while you're making them by giving you feedback in the left gutter. With linters in sublime text 3 we have to install the linters through package control. The creator of SublimeLinter decided that we're going to only use linting that you have natively installed so we'll actually have to install linting on the command line as well. That way, sublime text's understand of the languages wouldn't be behind any updates made to the languages. You can imagine that it be hard for one developer to update his package every single time any language changes what its syntax is.


- install sublime linter
- install linter jshint
- terminal: npm install -g jshint
- if you're using zshell, you **have** to include nvm in your zshenv file

- install linter csslint
- npm install -g csslint

- install linter htmltidy
- brew install tidy-html5

- install inter coffeelint
- npm install -g coffeelint



###### Git Gutter

Another one of my favorite packages is called Git Gutter. The display is when you've modified added or removed lines in a file since you last committed your work.

I find it extremely helpful to understand exactly what I've modified as I'm attempting to correct bugs. This one's easy—just install it through package control and it works.

###### Git

We can also install Git for sublime text. Mostly what I use Git for—within Sublime—is to use Git blame.

Once it's installed we can highlight a line that we want more information about, open our command palette and type blame. Git blame shows you the last person who modified that line. We find it extremely useful on the {{client}} team because it can help you get history and understand the intentions of the line you're looking at. We aren't really using it to say hey what the hell why'd you do that. Every team I've been on razor fish is very collaborative and I hope that that spirit is the same throughout all the offices. We encourage you to ask questions and we don't want you to spin your wheels trying to understand something that somebody else could tell you in 5 minutes.

###### Emmet

Alright moving on. This next one's a little bit different. It's called Emmet. It essentially allows you to use abbreviated HTML and CSS to reduce the amount of time that you spend typing. Let's install it with package control.

Cool now that it's installed, I'll open up a file, tell it that it's HTML (note that you don't have to do this if you actually want to save the file, thus giving it an extension), and I'll types some abbreviated HTML.

p turns straight in the paragraph
UL turns straight into an unordered list

The syntax here is a little bit different and I invit to go play with it. We are really going to cover much of it here but as the type of thing that you can do when you want to.

ul>li[class="item"]*8

You'll see that when it expands its places your cursor within somewhere that it thinks you probably want to edit. Heading tab will take you to the next one of those places automatically.

This works with CSS as well. I've gotten pretty accustomed to using things like "w100p" tab. Lowers the amount of manual typing you have to do, reduces errors.

###### Text Pastry

There's one other plug-in that I want to make a note of. It's a huge deal, but it's pretty cool. It is called text pastry.

The thing I like most about Text pastry is the ability to iterate when I have multiple cursors. So if I've taken a series of List items for example, and I decided that I want to make them numbered, usually you have to type a number on every single line manually, but with this we can just call a command have a stick in those numbers in order.

That kind of thing comes in a lot more handy when you're doing documentation, or if you're just trying to create an example for a codepen and need a quick way to assign for and ID on your inputs.

**{{Demo this with emmett}}**

___

{{if time, show a super fast cute video?}}


## Documentation

Alright next on the plate is documentation.

### Commenting in Sublime

Before we hit Markdown, I want to point out that you can create a line comment and sublime text with command plus /, or a block comment with command plus shift plus /. Remember that, and you don't need to remember the syntax for various languages.

I'm not really going to get into document blocks or anything like that here. But, I do want to say that I've never been a project that would've been worse off with more documentation. We should all be minifying our output before it actually goes out the door, so the comments you write are only going to be seen by your peers and anybody else that comes after to alter this code. Stay away from using language that you wouldn't want client to see, but don't hesitate to explain something weird that you've done. Often I find that intention behind what you write needs to be preserved even if the code needs to be modified, so if you find yourself needing to use magic numbers in CSS, or creating relationships between objects that only work if all three things are "just-so", please just call that out. You have to protect the code you write. You have to protect the intention behind it. And oftentimes even if somebody uses git blame and comes and asks you about it, you might've written it so long ago you don't even remember. So document it. No matter what the style, try to document it.

### Markdown

Okay so, markdown is a language that is used on github and stack overflow and superuser forums, and it's at least my language of choice for writing down release notes or other forms of documentation that you might have to then converted to PDF and send to the client.

- stackedit.io

When I'm using markdown and sublime text there're three packages that I prefer to install.

#### Markdown Editing

The first is called markdown editing. It provides syntax highlighting and slight adjustments on how the cursor behaves.

After installing mark done editing you're going to end up with this like text on white background sort of scheme. That can be adjusted though.

(When you install Markdown Extended, make sure you don't already have a Markdown file open.)

Okay, so it's default color is... well, I consider it awful.

You can go to Sublime Text > Preferences > Package Settings > Markdown Editing and then choose a user file there to reset it. You have three different syntaxes that this happens in, and will probably want to update all of them.

My preference? Monokai Extended.

#### Syntax

Let's take a minute to look at the syntax of markdown.

Paragraphs are created naturally simply by using linebreaks. You can create headings by using #'s to denote the level of heading. You can italicize by wrapping a word in _ or *. Add another _ or * to make it bold. Add another to make it bold and italic.

We can use - to create list items.

If we want to list indent within our list, we line break, indent, and use - again.

Using backticks, we can wrap something in a `code` tag.

If we want pre-formatted code, we indent the code block.

To create a link, we his [ and ] for the content of the link, and ( and ) for the href.

That's pretty much all we need know, so let's install a package that'll let us see the output. You see, everything you write and markdown converts into HTML.

#### Markdown Preview

Markdown preview is a package that parses markdown and opens it in your web browser.

Simply open up the command palette and type preview. Gives you options for whether or not you want to use hope flavored are done which allows for automatic code syntax highlighting but sends it to github's server in order to do so, or if you'd prefer standard markdown.

Let's go with standard markdown.

Cool.

#### Markdown TOC

Sometimes I find myself writing pretty long markdown files, we're just wanting to give a brief look at what's in store in the file very top. I don't do this by hand.

Mark down TOC is a plug-in that will create a table of contents in your markdown file based on the headings of the document.

We install it with package control, and then place it within our document with the command palette.

Now every time until the command pallet to update or every time you hit save on your file this will automatically update.

The only thing that I found I wish this did is create links to jump to the associated heading.

#### Mou

If you want a constant preview of what your markdown will output while you write it, there's an app for OS X called Mou. It's free, it's pretty nifty, but I have found it to be slow on longer documents, and generally once you understand the syntax, you don't need to constantly look at the output while you're using markdown.

___

{{another small cute video}}

## SourceTree

Alright, so let's get into source tree.

Source trees is developed by Atlassian, the same company that creates JIRA.

It is a visual interface for interacting with Git and Mercurial. Its free and frankly it's a step above the github app that does mostly same thing.

I personally find it a lot faster and more understandable then using the command line interface, I've also found that these tools are generally not that trusted by people who were really in the commandline and so this is a controversial application. But... haters gonna hate.

### Introduction to the Interface

So the first thing we will need to do an sorcery is at our repo to source tree. If you already cloned your repo, great! No need to do it again. Just hit new repository and choose the folder that you're .git file lives in.

etc.

- visualization of changes made
- visualization of branches
- toggling which branches you see in the Graph/Commit History

### Basic Tasks

#### Cloning a Repo (or adding an existing one)

#### Adding a Remote

#### Committing/Pulling/Pushing

##### Discard Hunk
##### Reset File
##### Cherrypicking

#### Branching

- Using folders

#### Merging

##### Coping with Merge Conflicts

### Advanced Tasks

#### Git Log

#### Git Blame
(I actually prefer to do this in Sublime, though)

#### Interactive Rebasing

#### Rebasing (ONLY ON YOUR LOCAL BRANCH)