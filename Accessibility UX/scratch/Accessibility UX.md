# Accessibility UX

2015 07 15 4–5pm

<!-- MarkdownTOC depth=6 -->

- About Accessibility
	- Your users / New User Personas
		- Hearing Disabilities (Deafness and Hard-of-Hearing)
		- Motor Disabilities (Physical impairments)
		- Visual Disabilities (Blindness and Low Vision)
		- Cognitive Disabilities
- Straight up copy/pasta'ed from MIT:
	- The obligatory POUR portion
		- Perceivable
		- Operable
		- Understandable
		- Robust
		- Just did POUR
- A Screen Reader's Experience
	- The Importance of a One to One Experience
	- Scanning: Landmarks and Headings
		- Types of Landmarks
		- How Heading Levels Work
		- Skip To Link
	- The Importance of a Linear Experience
- Staying Focused
	- Don't redirect focus
	- The Importance of Obvious Focus States
- pushing the limits within the limits
	- SPA difficulties
	- responsive difficulties
		- stray from Giving Elements Identity Crisis
- Misc - for design
	- Color Contrast
- Prototyping
- Component Patterns for the Web
	- Forms
		- Input types
	- Radios and checkboxes
		- Naming Conventions
		- Error Messaging
		- Tooltips
	- Tables
- Components WIP
	- Accordion
	- Alert
	- Alert or Message Dialog
	- Autocomplete
	- Button
	- Checkbox
		- Tri-State Checkbox
	- Combobox
	- Datepicker
	- Dialog_modal
	- Dialog_nonmodal
	- Dialog_tooltip
	- Draganddrop
	- Grid
	- Sortablegrid
	- Landmarks
	- Link
	- Listbox
	- Mediaplayer
	- Menu
	- Menubutton
	- Popupmenu
	- Popuphelp
	- Radiobutton
	- Richtext
	- Site_navigator_general
	- Site_navigator_tree
	- Site_navigator_tabbed_style
	- Slider
	- Slidertwothumb
	- Spinbutton
	- Tabpanel
	- Toolbar
	- Tooltip
	- Treegrid
	- Treeview
	- Windowsplitter
	- Wizard
	- Dropdown Menus
	- Modals
	- Expandable Content
	- Show More...
	- Replaceable content

<!-- /MarkdownTOC -->

___

## About Accessibility

### Your users / New User Personas

> Consider creating user personas for these

#### Hearing Disabilities (Deafness and Hard-of-Hearing)

> This is Smash. Smash used to be in a metal band and had the most wicked cabinets around. Now, when he's browsing videos on YouTube, he's always got the closed captions on.

Users with hearing impairments can use the web if provided captions for multimedia content (any video content that also has audio) and transcripts for audio-only content.   Without captions or transcripts, only the visual content is accessible.

#### Motor Disabilities (Physical impairments) 
Users with motor impairments are more likely to use only a mouse, only a keyboard, voice or other inputs to control and navigate the web.   Websites developed with flexibility of input options are more accessible to these individuals.  Requiring mouse-only or keyboard-only control will create a barrier for some of these individuals.

#### Visual Disabilities (Blindness and Low Vision)
Users with vision loss can rely on screen enlargement, keyboard-only navigation, and/or the use of screen reader technology.  Access to information via these means is dependent on: sizable fonts, good color contrast, and well-structured websites that label all graphics, icons, buttons, and multimedia, using web standards for coding tables, forms, and frames. 

#### Cognitive Disabilities
User with cognitive impairment rely on consistent navigation structure. Overly complex presentation, flickering or strobing designs can be confusing to these users.


>
	- the blind
	- the not-blind
	- the partially blind
	- the color blind
	- the physically impaired
	- keyboard users
	- your grandparents
	- people with no patience
	- and me


## Straight up copy/pasta'ed from MIT:

[MIT - UX Accessibility Guidelines](https://ux.mit.edu/accessibility/guidelines)

### The obligatory POUR portion

I'd be remiss to miss this.

#### Perceivable

Content is Perceivable in multiple ways

- Audio content is captioned for those that cannot perceive the audio through hearing alone.
- Text alternatives are provided for non-text content.
- State changes—focus, interactions... you should be getting feedback

#### Operable

Content is Operable by multiple means

It gotta work.

Whether you're on keyboard only, touchscreen, etc
- All functionality is available through the keyboard only
- Users can navigate and find information easily

#### Understandable

Content is Understandable

​- Text is readable and understandable
- Content appears and is operable in **predictable** ways

#### Robust

Offerings are Robust across multiple platforms

- Site interacts with standard mobile devices and assistive technologies

#### Just did POUR

**These four ideals/features create the common acronym POUR, which you'll see in nearly any beginner level accessibility tutorial.**

## A Screen Reader's Experience

- VoiceOver for OS X
	- `Command` + `F5`
	- can navigate from element to element
	- can navigate by element type
- VoiceOver for iOS
	- typically swiping from element to element
	- can also navigate by types of elements
	- can also point at elements

NVDA and Talkback aren't terribly different from these two. NVDA gives the user the ability to hear items they're hovering over as well.

### The Importance of a One to One Experience

Because we can interact with the page in so many ways, it's important that we structure the page in a manner that makes these interactions useful.

Everything ~important~ (non-decorative) you are able to see, you should be able hear, you should be able to reach out and touch it, hover over it (if supported), click on it (and navigate to it with keyboard alone) if it's actionable, etc.

Similarly, nearly everything you hear should have a visible on-page component that's related to it. An X icon may say "Close", an image may be described, a tooltip may say "Open tooltip" when these words aren't present on the page, but the user should understand what visible object is being read. We should not be hiding entire passages of text just for a screen reader, because, well, how likely are you to point at it and see it? There's no spirit realm here. We just want to make this stuff exist in nearly every percievable way it can.


### Scanning: Landmarks and Headings

Users generally rely on headings and landmarks to scan the page.

- landmarks allow them to jump from area to area
- within these areas, it's best that the experience is linear

#### Types of Landmarks

#### How Heading Levels Work

#### Skip To Link

- jumping past redundant elements and navigation, etc. — screen readers already have this ability. At this point, it's mainly for keyboard users, so making the link visible when it's focused is a good idea

### The Importance of a Linear Experience

- element order, within a module/component, is arranged left-to-right top-to-bottom (assuming it's an English page).
- information that's necessary to the user should be presented in a logical and upfront manner. Close your eyes and walk through this. Did you have all the information you needed to have to make a sound judgement on whether or not to submit this form?
	- EXAMPLE: form with Terms and Conditions below the Submit button "your email address is optional. If you give us your email address, we will send you offers from our partners."

## Staying Focused

- we always have to keep track of a user's focus
	- don't instantly place them on elements because they can miss information
		- EXAMPLE: instantly focused find field
	- no locking them on elements
		- EXAMPLE: a worse focused find field

### Don't redirect focus

- EXAMPLE: three input fields for phone number

### The Importance of Obvious Focus States

- focus states focus states focus states
	- embrace these. make them cool!




___
___







## pushing the limits within the limits

### SPA difficulties

At this point in time, the ideal screen reader experience is a page that has true separate page loads.

### responsive difficulties

https://medium.com/salesforce-ux/7-things-every-designer-needs-to-know-about-accessibility-64f105f0881b

#### stray from Giving Elements Identity Crisis

- minor design changes could lead to changes in a user’s interaction model.
- thou shalt not switch input types - breaks our STAYING FOCUSED rule



## Misc - for design

### Color Contrast
	- there be standards for compliance
	- your icons don't matter—actually, all that matters is text on a background
		- so this (pic of text on a crazy background) is bad

## Prototyping

Prototyping accessibility for the web requires knowledge of established patterns. Anything new requires testing.

## Component Patterns for the Web

http://www.w3.org/TR/wai-aria-practices/#aria_ex

### Forms

- where to place important information
- the expectation of being able to tab through an entire form
- creating related content
	- fieldsets and how they sound

#### Input types

### Radios and checkboxes

Issues with overlaying native elements
- try selecting this radio button/checkbox by hovering over it


##### Naming Conventions
##### Error Messaging
##### Tooltips

- multiple constraints:
	- we can either treat these as modals
	- or have them read immediately

### Tables

so tricky.


___

## Components WIP

From http://www.w3.org/TR/wai-aria-practices/#aria_ex

### Accordion

http://www.oaa-accessibility.org/examplep/accordian1/

### Alert

http://www.oaa-accessibility.org/examplep/alert1/

### Alert or Message Dialog

http://www.oaa-accessibility.org/examplep/alertdialog1/

### Autocomplete

http://archive.dojotoolkit.org/nightly/dojotoolkit/dijit/tests/form/_autoComplete.html

- doesn't work very well at all in Chrome VO

### Button

- care for all states

https://css-tricks.com/so-many-states/

- toggle buttons


### Checkbox

- these require basically rewriting native components entirely

http://www.oaa-accessibility.org/examplep/checkbox2/

#### Tri-State Checkbox

### Combobox

http://www.oaa-accessibility.org/examplep/combobox2/
http://www.oaa-accessibility.org/examplep/combobox5/

### Datepicker

May or may not work at all. Doesn't function in Chrome.

DO: have a separate date field from button that allows user to open the picker itself

http://www.oaa-accessibility.org/examplep/datepicker1/

### Dialog_modal

We've done this best.

Incredible Accessible Modal

### Dialog_nonmodal


### Dialog_tooltip


### Draganddrop


### Grid


### Sortablegrid


### Landmarks


### Link


### Listbox


### Mediaplayer


### Menu


### Menubutton


### Popupmenu


### Popuphelp


### Radiobutton


### Richtext


### Site_navigator_general


### Site_navigator_tree


### Site_navigator_tabbed_style


### Slider


### Slidertwothumb


### Spinbutton


### Tabpanel


### Toolbar


### Tooltip


### Treegrid


### Treeview


### Windowsplitter


### Wizard








___



### Dropdown Menus


### Modals

### Expandable Content

- it's best to keep the button that expands content 

### Show More...

- ick

### Replaceable content

