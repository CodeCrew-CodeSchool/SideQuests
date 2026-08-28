# Day 4 - HTML Forms, Links, and Media

## Overview

Today I learned how HTML can do more than just display information. I worked with forms to collect information from users, linked multiple HTML pages together, used images, and embedded YouTube videos with `iframe`.

I also got more practice understanding HTML attributes and file paths.

---

## HTML Forms

A `<form>` is used to collect information from a user.

Example:

```html
<form action="mailto:example@email.com" method="post" enctype="text/plain">
</form>
```

### Form Attributes

- `action` - tells the form where the submitted information should go
- `mailto:` - tells the browser to open an email application
- `method="post"` - sends the information as submitted form data
- `enctype="text/plain"` - formats the submitted information as plain text

A simple pattern to remember:

```html
<form action="WHERE IT GOES" method="HOW IT SENDS" enctype="FORMAT">
```

---

## POST

`POST` is an HTTP method used when submitting information.

A simple way to think about it:

- `GET` - usually retrieves or asks for information
- `POST` - usually sends or submits information

With `GET`, information can sometimes appear in the URL.

With `POST`, the information is sent as part of the request instead.

---

## Labels

The `<label>` element tells the user what an input is asking for.

Example:

```html
<label for="email">Email:</label>
```

Breaking it down:

- `<label` - starts a label
- `for="email"` - connects the label to an element with `id="email"`
- `Email:` - the text the user sees
- `</label>` - closes the label

### Label Pattern

```html
<label for="x">Visible Text:</label>
```

The `for` value should match the `id` of the input it belongs to.

---

## Input Fields

The `<input>` element allows the user to enter information.

Example:

```html
<input type="email" id="email" name="email">
```

Breaking it down:

- `type` - determines what kind of input it is
- `id` - identifies the input and connects it to its label
- `name` - gives the submitted data a name

### Input Pattern

```html
<input type="kind" id="x" name="x">
```

Example:

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name">
```

The connection is:

```text
for="name"
     ↓
id="name"
```

---

## Input Types

Different `type` values create different kinds of inputs.

Examples:

```html
<input type="text">
<input type="email">
<input type="password">
<input type="number">
<input type="checkbox">
<input type="radio">
```

`type="text"` is used for normal text.

`type="email"` tells the browser that an email address is expected.

---

## Textarea

`<textarea>` is used for longer messages or information that may need multiple lines.

Example:

```html
<textarea id="message" name="message"></textarea>
```

Unlike `<input>`, `<textarea>` has an opening and closing tag.

Its starting size can also be changed:

```html
<textarea rows="4" cols="40"></textarea>
```

- `rows` - approximate height
- `cols` - approximate width

---

## Required Attribute

The `required` attribute tells the browser that a field must be filled out before the form can be submitted.

Example:

```html
<input type="email" required>
```

`required` does not need a value.

The browser can automatically warn the user if they try to submit the form without completing that field.

---

## Submit Button

A button can be used to submit a form.

```html
<button type="submit">Submit</button>
```

`type="submit"` tells the browser to submit the form that the button is inside.

---

## Line Breaks

`<br>` means **line break**.

It moves whatever comes next onto a new line.

Example:

```html
<label for="name">Name:</label>
<br>
<input type="text" id="name">
```

This appears more like:

```text
Name:
[__________]
```

Two line breaks:

```html
<br><br>
```

create an extra blank line.

`<br>` does not need a closing tag.

---

## Contact Form Assignment

I created a basic Contact Me form with:

- Name input
- Email input
- Message textarea
- Submit button
- `mailto:` action

The main structure looked like:

```html
<form>
    <label></label>
    <input>
    <textarea></textarea>
    <button></button>
</form>
```

One useful way to think about forms is:

```text
User → Information → Website
```

Earlier HTML was mostly:

```text
Website → Information → User
```

Forms allow the user to start sending information back.

---

# Links

The `<a>` element creates a link.

Example:

```html
<a href="mauiAdventure.html">Scuba Diving in Maui</a>
```

Breaking it down:

- `<a>` - creates the link
- `href` - tells the browser where to go
- the text between the tags is what the user clicks

### Link Pattern

```html
<a href="destination">Clickable Text</a>
```

When linking to another HTML file, the filename has to match the real filename.

For example:

```html
<a href="mauiAdventure.html">Maui</a>
```

only works if the file is actually named:

```text
mauiAdventure.html
```

A typo or different filename can cause a "page does not exist" error.

---

## Multi-Page Websites

I created a website with multiple HTML files:

```text
index.html
mauiAdventure.html
yellowstoneAdventure.html
```

The homepage linked to the two adventure pages.

```text
               index.html
                    |
         ┌──────────┴──────────┐
         ↓                     ↓
mauiAdventure.html   yellowstoneAdventure.html
```

This helped me understand how separate HTML files can work together as one website.

---

# File Paths

HTML uses file paths to find other files in a project.

Example project:

```text
project/
│
├── index.html
├── mauiAdventure.html
├── yellowstoneAdventure.html
│
└── images/
    └── maui.jpg
```

To use the image from `index.html`:

```html
<img src="images/maui.jpg" alt="Outdoor adventure">
```

The browser reads that path like:

```text
index.html
   ↓
images
   ↓
maui.jpg
```

---

# Images

Images use the `<img>` element.

```html
<img src="images/maui.jpg" alt="Outdoor adventure">
```

- `src` - tells the browser where the image is located
- `alt` - gives the image a description

`alt` is useful for accessibility and also gives information if an image cannot load.

`<img>` does not need a closing tag.

---

# Image Formats

## JPG / JPEG

Good for:

- photographs
- detailed images
- smaller file sizes

JPG uses compression, so some image information is lost.

## PNG

Good for:

- graphics
- logos
- screenshots
- transparent backgrounds

PNG is lossless, meaning it preserves image information better, although the files can be larger.

## GIF

Good for:

- simple animations

GIF supports a limited number of colors, so it is usually not the best format for detailed photographs.

---

# iframe

An `<iframe>` lets another webpage or media player appear inside an HTML page.

Example:

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="Video Title">
</iframe>
```

A normal YouTube URL might look like:

```text
https://www.youtube.com/watch?v=gHcnzz5Nyxg
```

For an iframe, the embed URL looks like:

```text
https://www.youtube.com/embed/gHcnzz5Nyxg
```

The video ID stays the same.

```text
watch?v=
```

changes to:

```text
embed/
```

I think of an iframe as a small window that displays content from another webpage inside my webpage.

---

# Outdoor Adventures Assignment

I created a multi-page outdoor adventure website.

The homepage included:

- An `Outdoor Adventures` heading
- An outdoor image
- A link to the Maui page
- A link to the Yellowstone page

The Maui page included:

- `Scuba Diving in Maui` heading
- Embedded YouTube video
- Short paragraph about the adventure

The Yellowstone page included:

- `Hiking in Yellowstone` heading
- Embedded YouTube video
- Short paragraph about the adventure

This assignment gave me more practice with:

- `<a>`
- `href`
- `<img>`
- `src`
- `alt`
- `<iframe>`
- `<p>`
- File paths
- Multiple HTML files

---

# New HTML Element I Researched

I also learned about the `<details>` element.

`<details>` creates a section that the user can open and close.

Example:

```html
<details>
    <summary>More Information</summary>
    <p>This information appears when the section is opened.</p>
</details>
```

This could be useful for:

- FAQs
- Instructions
- Extra information
- Content that does not always need to be visible

---

# Git Notes

I continued using VS Code Source Control to commit my work.

I also ran into this error:

```text
fatal: not a git repository
```

This means my terminal was not currently inside the cloned Git repository.

Useful commands:

```bash
pwd
```

Shows the current folder.

```bash
ls
```

Shows files and folders in the current location.

```bash
cd folder-name
```

Moves into another folder.

```bash
git status
```

Shows the status of the current Git repository.

Git commands need to be run inside the cloned repository or one of its folders.

---

# Day 4 Takeaways

Today I learned:

- How HTML forms work
- How `<form>` acts as a container
- How labels connect to inputs
- The difference between `type`, `id`, and `name`
- What `POST` means
- How to use `<textarea>`
- How `required` provides simple form validation
- How submit buttons work
- What `<br>` does
- How `<a>` and `href` create links
- How multiple HTML files become a multi-page website
- How file paths work
- How to display images
- The differences between JPG, PNG, and GIF
- How to embed YouTube videos using `<iframe>`
- How small filename mistakes can break links
- How to recognize when the terminal is not inside a Git repository