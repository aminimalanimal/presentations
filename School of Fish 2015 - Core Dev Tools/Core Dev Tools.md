# Core Dev Tools and Process

<!-- MarkdownTOC depth=6 -->

- Overview
	- Criteria for Success
- Sublime Text
	- Interface Basics
		- Navigating
			- Side Bar
			- Goto Anything
			- Find
		- Columns
		- Word Wrap
		- Working with Multiple Cursors
		- Copy/Pasta
	- Commenting
		- Command Palette
	- Customizing Your Sublime Workflow
		- Preferences
		- Plugins
			- Installing Package Control
			- Syntax Highlighters
			- Linters
			- Emmet
			- Git
			- Git Gutter
			- Gists
			- Color Highlighter
			- Text Pastry
		- Snippets
	- Overall Demonstration
- Documentation
	- Introduction to Markdown
	- Package: Markdown Editing
	- Package: Markdown Preview
	- Package: Markdown TOC
- SourceTree
	- Introduction to the Interface
	- Basic Tasks
		- Cloning a Repo (or adding an existing one)
		- Adding a Remote
		- Committing/Pulling/Pushing
			- Discard Hunk
			- Reset File
			- Cherrypicking
		- Branching
		- Merging
			- Coping with Merge Conflicts
	- Advanced Tasks
		- Git Log
		- Git Blame
		- Interactive Rebasing
		- Rebasing (ONLY ON YOUR LOCAL BRANCH)
- Other Misc Tools
	- Regexr
	- Moom
- Debugging (Only if there's time)
	- Chrome Dev Tools
		- Elements
		- Network
		- Sources
		- Resources
		- Parallels/VMWare/Virtual Box/Browserstack
		- Debugging iOS
		- Debugging Android

<!-- /MarkdownTOC -->

## Overview

Sublime Text, SourceTree, and Documentation with Markdown

This course is all about introducing tools that will make your lives as developers easier.

**Never underestimate tiny gains in efficiency**

With Sublime Text, you'll learn to rapidly find what we're looking for in large projects—and who wrote it, write code faster and cleaner, reduce errors with syntax highlighting, linters, and git integration.

With SourceTree, you'll learn to perform most Git operations free of command line, allowing you to easily overview code changes and prepare clean commits you can feel confident in.

With Markdown, you'll learn to document and write about code—allowing you to communicate gracefully in GitHub, StackOverflow, README files/etc.

### Criteria for Success

The students are expected to recognize the types of tools at their disposal that will allow them to increase efficiency with their code editor and source control, reduce errors while writing code, document their code to communicate their intentions.


## Sublime Text

### Interface Basics

#### Navigating

##### Side Bar

- `command` + `k`, `b`

##### Goto Anything

- `command` + `p` - Goto Anything - fuzzy search!
	- type in parts of name, even the path

##### Find

- `command` + `shift` + `f`
	- what the little tools mean
	- how to only search certain files with `*.jade`, `*.coffee`

- `command` + `i` - incremental search

#### Columns

- `command` + `option` + `1`/`2`/`3`/`4`

#### Word Wrap

- `View` > Word Wrap

#### Working with Multiple Cursors

- `command` + click
- `command` + `d`
- `control` + click and drag - column selection

Through OS X, but especially helpful here:

- navigating with `option` + `<-` / `->`
- navigating with `command` + `<-` / `->`

#### Copy/Pasta

- copy whole line just by being on the line
	- with multiple cursors, copying whole line will cause all lines to be placed in multiple places
- copying part of line
	- each cursor will rememeber only it's portion

- `command` + `shift` + `v` (inline paste)
- `control` + `shift` + `^`/`V`

Shifting indentation manually:

- `command` + `[` / `]`
- switching between tabs and spacing, setting it in preferences

### Commenting

- `command` + `/`
- `command` + `shift` + `/`

#### Command Palette

- `command` + `shift` + `p`
- you can find anything here

### Customizing Your Sublime Workflow

#### Preferences

- yours go in Preferences > User
- just json
- how to set new preferences
- here's a bunch of possible preferences, and things I like

#### Plugins

##### Installing Package Control

Let's take a minute to install Package Control. It's the only package you'll have to install manually.

##### Syntax Highlighters

- install syntaxes
- browse through syntaxes

##### Linters

- how to install
	- walk through terminal installation for javascript linter
	- install package

##### Emmet

- superfast HTML and CSS!

##### Git

- mostly to Git Blame

##### Git Gutter

- what the signs mean, how awesome this is

##### Gists

- creating gists
- updating
- using gists as snippets

##### Color Highlighter

- see colors just by clicking on them

##### Text Pastry

- instant iteration!

#### Snippets

- demo javascript `if`, `for`, `func` stuff
- how to create snippets
	Tools > New Snippet
	- `.sublime-snippet`
- explain tab stops ${1:this}
- demo snippet creation
	- src snippet
	- style snippet

### Overall Demonstration










## Documentation

### Introduction to Markdown

	There's no such thing as self-documenting code.
	Bugs will happen, and will often be corrected by other developers. 
	Protect your intentions with documentation.

Documentation is going to be a big part of your job, if you're good at it. I suggest taking an interest in it.

### Package: Markdown Editing

### Package: Markdown Preview

- also note: Mou

### Package: Markdown TOC

- instant table of contents!
- just use `depth=n`










## SourceTree

### Introduction to the Interface

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

___

## Other Misc Tools

### Regexr

### Moom

___

## Debugging (Only if there's time)

### Chrome Dev Tools

#### Elements

I assume you've used this. Got CSS, the ability to copy/edit HTML, etc.

You can also:

- force element state

#### Network

- clear
- filter!

Need to find something? Filter: can choose elements types

This is really handy for finding json that gets passed back and forth, and finding the original state of a webpage before javascript performs DOM manipulation on it.


#### Sources

JavaScript debugging land!

- breakpoints
	- step over
	- step into
	- okay, let's step out of jQuery
	- oh crap! we're in jQuery! time to cut jQuery out of it
	- difference between the play buttons
- using the console along with being paused
	- scope variables and watch expressions
	- call stack

#### Resources

See all the document types in one place


#### Parallels/VMWare/Virtual Box/Browserstack

#### Debugging iOS

- use Safari or WebKit
- make sure you have Apple Developer Tools installed through XCode

#### Debugging Android

- use Chrome
