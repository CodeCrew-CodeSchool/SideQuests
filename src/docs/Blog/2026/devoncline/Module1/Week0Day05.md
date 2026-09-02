# Day 5 - More HTML

## Building a Multi-Page Website

Today I worked on a larger HTML project that expanded on what I learned earlier in the week.

Instead of creating a single webpage, I created a website with three separate pages:

- `index.html` - About Me
- `myHobbies.html` - My Hobbies
- `myFavoriteEats.html` - My Favorite Eats

Each page has navigation links that allow the user to move between the different pages.

## Internal and External Links

I practiced using the anchor tag to create both internal and external links.

An internal link connects to another page within the same website:

`<a href="myHobbies.html">My Hobbies</a>`

An external link connects to another website:

`<a href="https://github.com/">GitHub</a>`

The `href` attribute tells the browser where the link should go.

I also learned that when HTML files are inside the same folder, I can link directly to the filename instead of needing a full URL.

## Semantic HTML

Today I used more semantic HTML elements to organize my pages.

Some of the semantic elements I used were:

- `<header>` - contains introductory content at the top of a page
- `<nav>` - contains navigation links
- `<main>` - contains the main content of the page
- `<section>` - groups content that belongs to a specific section

These elements usually do not change how the website looks by themselves. Their purpose is to give the HTML more structure and meaning.

For example:

`<nav>` tells the browser that the links inside it are being used for navigation.

A `<div>` can also group elements together, but it does not describe what that group represents.

## Lists

I used an unordered list to organize my hobbies and favorite foods.

`<ul>` creates an unordered list.

Each item inside the list uses an `<li>` tag.

Example:

`<ul>`
`    <li>Music Production</li>`
`    <li>Software Development</li>`
`    <li>Gaming</li>`
`</ul>`

I also learned that an `<li>` can contain more than just text. It can contain headings, images, paragraphs, links, and other HTML elements.

## Images

I added several images using the `<img>` tag.

Example:

`<img src="Images/example.jpg" alt="Description of image" width="400">`

The `src` attribute tells the browser where the image file is located.

The `alt` attribute provides a description of the image. This is useful for accessibility and also provides information if the image cannot load.

I also learned that file and folder capitalization can matter when a website is hosted online, so paths such as `Images/` and `images/` should be used consistently.

## Embedded Video

I practiced embedding a YouTube video using an `<iframe>`.

Example:

`<iframe width="560" height="315" src="YOUTUBE-EMBED-URL" allowfullscreen></iframe>`

An iframe allows content from another website, such as YouTube, to appear inside my webpage.

I also experimented with an Instagram embed and learned that some embeds depend on scripts from the external website and may behave differently than a normal YouTube iframe.

## Creating a Contact Form

I also created my first HTML contact form.

The form included fields for:

- Name
- Email
- Message
- Submit button

Some of the new elements I used were:

`<form>` - groups the form elements together

`<label>` - tells the user what information an input is asking for

`<input>` - creates an input field

`<textarea>` - creates a larger box for multi-line text

Example:

`<label for="email">Email:</label>`

`<input type="email" id="email" name="email">`

The `for` attribute on the label matches the `id` of the input. This connects the label to that specific input field.

I also learned that different input types can tell the browser what kind of information should be entered, such as:

`type="text"`

or

`type="email"`

## HTML vs CSS

I used `<br>` tags to create some line breaks and spacing in my form.

I learned that while this works, CSS will eventually be the better way to control spacing and layout.

A useful way to think about it is:

- HTML = structure and content
- CSS = appearance and layout
- JavaScript = behavior and interactivity

For now, I am mainly building the structure of the website with HTML. I will be able to improve the design later when we begin learning CSS.

## VS Code Tips

I learned a few VS Code shortcuts that make editing HTML easier.

### Format Document

`Shift + Alt + F`

This automatically formats the document and fixes things like indentation and spacing.

### Indent Selected Lines

`Tab`

Moves selected lines to the right.

### Unindent Selected Lines

`Shift + Tab`

Moves selected lines back to the left.

I also learned about **Emmet: Wrap with Abbreviation**, which can wrap existing HTML inside another element without manually moving everything.

## What I Built Today

By the end of the day, I had a three-page About Me website containing:

- Navigation between pages
- Semantic HTML structure
- Headings and paragraphs
- Internal links
- External links
- Images
- Lists
- An embedded video
- A contact form

This project will continue to be expanded as I learn CSS and JavaScript.