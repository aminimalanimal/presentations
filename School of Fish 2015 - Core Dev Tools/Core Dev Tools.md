# Core Dev Tools and Process

<!-- MarkdownTOC depth=6 -->

- Criteria for Success
- OS X
- Sublime Text
	- Introduction to the Interface
	- Installing Package Control
	- Controls
		- Working with Multiple Cursors
			- Word Wrap
			- Package: Text Pastry
			- Demonstration
		- Lookin' fer stuff
		- Columns
	- Documentation: Markdown Support
		- Intro to Markdown
		- Package: Markdown Editing
		- Package: Markdown Preview
		- Package: Markdown TOC
	- Other Packages
		- Git Gutter
		- LINTERS
		- Color Highlighter
		- Syntax Highlighters
		- Emmet
- Debugging
	- Chrome Dev Tools
		- Elements
		- Network
		- Sources
		- Resources
	- Debugging iOS
	- Debugging Android
	- Parallels/VMWare/Virtual Box/Browserstack
- SourceTree
- Other Misc Tools
	- Regexr

<!-- /MarkdownTOC -->

~Never underestimate tiny gains in efficiency~

## Criteria for Success

The students are expected to recognize the types of tools at their disposal that will allow them to increase efficiency with their code editor and source control, reduce errors while writing code, document their code to communicate their intentions, and debug css, javascript, json (iOS, IE, Android) within a browser.

Students will be able to know where to go to find additional resources.

## OS X

- navigating with `option` + `<-` / `->`
- navigating with `command` + `<-` / `->`





## Sublime Text

### Introduction to the Interface

- side bar (though you may not need it much)
- preferences panel, and how to set new preferences
	- yours go in Preferences > User
	- just json
	- here's a bunch of possible preferences, and things I like

### Installing Package Control

Let's take a minute to install Package Control. It's the only thing you'll have to do manually.

### Controls

Doin' things - the thing-doer command

- `command` + `shift` + `p`
- `command` + `shift` + `v` (inline paste)
- `command` + `[` / `]`
- `command` + `option` + `1`/`2`/`3`

#### Working with Multiple Cursors

- `command` + click
- `command` + `d`
- `control` + `shift` + `^`/`V`
- `control` + click and drag - column selection

##### Word Wrap

- `View` > Word Wrap

##### Package: Text Pastry

- instant iteration!

##### Demonstration

(Come up with quick demo, multiple fields, numbers, ids, etc.)


#### Lookin' fer stuff

- `command` + `shift` + `f`
	- what the little tools mean
	- how to only search certain files with `*.jade`, `*.coffee`
- `command` + `p` - Goto Anything - fuzzy search!
	- type in parts of name, even the path


- `command` + `i` - incremental search

#### Columns

- `command` + `option` + `1`/`2`/`3`/`4`

### Documentation: Markdown Support

#### Intro to Markdown

	There's no such thing as self-documenting code.
	Bugs will happen, and will often be corrected by other developers. 
	Protect your intentions with documentation.

Documentation is going to be a big part of your job, if you're good at it. I suggest taking an interest in it.

- note: this applies to Github as well.

#### Package: Markdown Editing

#### Package: Markdown Preview

- also note: Mou

#### Package: Markdown TOC

- instant table of contents!
- just use `depth=n`



### Other Packages

#### Git Gutter

- what the signs mean, how awesome this is

#### LINTERS

#### Color Highlighter

#### Syntax Highlighters

#### Emmet

- superfast HTML and CSS!





## Debugging

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



### Debugging iOS

- use Safari or WebKit
- make sure you have Apple Developer Tools installed through XCode

### Debugging Android

- use Chrome

### Parallels/VMWare/Virtual Box/Browserstack

## SourceTree

- The ease of cherrypicking


## Other Misc Tools

### Regexr
