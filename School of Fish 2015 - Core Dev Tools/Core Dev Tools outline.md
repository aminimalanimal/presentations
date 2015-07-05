# Core Dev Tools and Process

2015 07 15 morning

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
	- Customizing Your Sublime Workflow
		- Preferences
		- Command Palette
			- Plugins
				- Installing Package Control
				- Syntax Highlighters
				- Linters
				- Git Gutter
				- Git
				- Emmet
				- Text Pastry
				- Gists
				- Color Highlighter
		- Snippets
	- Overall Demonstration
- Documentation
	- Commenting in Sublime Text
	- Introduction to Markdown
	- Places where we can use Markdown
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
- `command` + `control` + `g`
- `control` + click and drag - column selection
- `control` + `shift` + `^`/`V`

Through OS X, but especially helpful here:

- navigating with `option` + `<-` / `->`
- navigating with `command` + `<-` / `->`

#### Copy/Pasta

- copy whole line just by being on the line
	- with multiple cursors, copying whole line will cause all lines to be placed in multiple places
- copying part of line
	- each cursor will rememeber only it's portion

- `command` + `shift` + `v` (inline paste)

Shifting indentation manually:

- `command` + `[` / `]`
- switching between tabs and spacing, setting it in preferences





### Customizing Your Sublime Workflow

#### Preferences

- yours go in Preferences > User
- just json
- how to set new preferences
- here's a bunch of possible preferences, and things I like

#### Command Palette

- `command` + `shift` + `p`
- you can find anything here

##### Plugins

###### Installing Package Control

Let's take a minute to install Package Control. It's the only package you'll have to install manually.

###### Syntax Highlighters

- install syntaxes
- browse through syntaxes

###### Linters

- how to install
	- walk through terminal installation for javascript linter
	- install package

###### Git Gutter

- what the signs mean, how awesome this is

###### Git

- mostly to Git Blame

###### Emmet

- superfast HTML and CSS!

###### Text Pastry

- instant iteration!

###### Gists

- creating gists
- updating
- using gists as snippets

###### Color Highlighter

- see colors just by clicking on them

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

### Commenting in Sublime Text

- `command` + `/`
- `command` + `shift` + `/`

### Introduction to Markdown

	There's no such thing as self-documenting code.
	Bugs will happen, and will often be corrected by other developers. 
	Protect your intentions with documentation.

Documentation is going to be a big part of your job, if you're good at it. I suggest taking an interest in it.

### Places where we can use Markdown

- stackedit.io
- stackoverflow/superuser
- github
- mou

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