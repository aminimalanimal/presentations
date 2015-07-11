# Accessibility UX elaborated

## Intro

Hi my name is James curd. I'm a presentation layer engineer here at the Austin office. I've worked here for about two years on the {{client name}} account. {{Client name}} recently revamped their entire website. One of the driving factors behind the rewrite was to make it accessible.

There is an increasing fear that the government will adopt an open-standards spec called the WCAG—the Web content accessibility guidelines— as it's official standard for compliance with the Americans with Disabilities Act that passed in 1990. The ADA prevents discrimination based on disability, and in recent years many companies that have functionality deemed to be universal enough to be a public service—such as banks and airlines—have found themselves under pressure to offer their services and their websites to everyone, lest they be sued.

So, my primary focus so far at Razorfish has been Web accessibility... but bear in mind that the takeaways here apply to everything. The ADA is why we have handicapped parking spots, wheelchair ramps, Braille in elevators, walk signs that beep and talk to you. Our public spaces have adjusted their layout, their design, and they're behavior in order to be more universally accessed. The web is no different.

Now frankly, your client may not be a bank or an airline. Your client may not come to you with this as a concern. And when it's not part of the clients agenda, the concessions can be hard to sell.

And... look—I say concessions, and I mean it. If you're making an accessible website, you simply cannot do all of the things that you might have done if you weren't. So, there are concessions, however, many of those concessions lead to a more positive experience for everybody.

### Mission Statement

Creating a truly accessible website requires a lot of knowledge. Not just from your developers, or your testers, but right in the beginning as well—from the functional requirements, the information architecture, and the design itself.

And even without buy-in from a client, there are certainly several steps we can take in the right direction, and they begin with awareness.

## Our Users

Let's talk about who our users are.

We're already used to thinking about different users.

People from different backgrounds, with different skill sets, with different understandings of technology are all going to interface with your products in a slightly different manner. Skeumorphism was so popular for so long because it was believed that people needed an interface analogous to real world objects they were already accustomed to.

We already design for simple users in mind. We design for power users. We design for people who have too much time on their hands, and for people who have no patience.

The first thing that most people think when they hear accessibility is that we are going to design for the blind. This was the mistake I made when I first started. It seemed to me like our website could have a representation for the sighted and another representation for the non-sighted. While we were always opposed to coding two separate websites for this, several of our techniques still adopted that mentality. That "oh—this bit of content is only for people who are blind" mentality, and it often caused the experience to differ.

It turns out that this was wrong because not all of our users are fully blind. There is no clear distinction between our sighted users and our non-sighted users. Most of the people that I've met that use screen readers are partially blind. They see certain colors with greater Visual clarity than others. They have specks in their vision. Warps. They can see but they have to put their face 6 inches away from screen. They can see but they have to keep their head 5 feet away from the screen. They can see but they're going to be accessing the site with a tool that zooms in they're looking at 16 times the size that you and I would look at it.
It's not just vision, though.

We design for iPhones, computers, tablets, video game consoles, displays in a mall or airport, etc, and so we're getting used to thinking about designing for mice and fingers and gestures.

We also need to design for for users who are accessing the computer only through a keyboard, relying solely on browser-based navigation like the tab key and up and down arrows.

We also need to design for people accessing the site through a screen reader, whose experience Will be determined by the semantic quality of the code, the hierarchy of our information, and how well we can present it linearly. The screen reader sits on top of the existing functionality and essentially allows users to hover over various parts of The website, and when they do that, it tells them what they are. So this limits our ability to use clever visual techniques to cover up things, to make them seem like they are something else, to transform them willingly.

We also need to care for deaf users. We need to provide closed captioning for audio content.

And we need to care for users with cognitive disabilities. We need to make sure the that language that we use is understandable—the lower the grade-point level of writing, typically, the better.

## The tenants of accessible design

You need to make sure that users can perceive our website. They understand where they're focuses That they understand what elements are, they can see the dividing lines between things, that they understand when an error has taken place.
The first tenant of accessible design is that you provide multiple ways to perceive everything. Now that's not as hard as it sounds. It actually just means that if you have a picture, you give it alt text. If you have an input, it's actually coded as an input, that way when a user uses a screen reader, they can hear that it is an input.