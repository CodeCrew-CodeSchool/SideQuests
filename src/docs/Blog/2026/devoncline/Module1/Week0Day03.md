# Day 3 - Introduction to HTML

## Intro to HTML

Today I started learning more about HTML and how it creates the structure of a webpage.

HTML stands for **HyperText Markup Language**. Unlike Markdown, HTML uses tags inside angle brackets (`< >`) to tell the browser what each piece of content is.

## Basic HTML Structure

When creating an `index.html` file in VS Code, I can type:

`!`

and press Enter/Tab to automatically generate the basic HTML structure.

This shortcut is part of **Emmet**, which is built into VS Code.

The generated structure includes things like:

- `<!DOCTYPE html>` - tells the browser that the document uses HTML5
- `<html>` - contains the entire HTML document
- `<head>` - contains information about the webpage that is not part of the main visible content
- `<meta>` - contains settings/information about the webpage
- `<title>` - controls the text shown on the browser tab
- `<body>` - contains the content that is actually displayed on the webpage

## HTML Elements and Tags

Most HTML elements have an **opening tag** and a **closing tag**.

Example:

`<p>This is a paragraph.</p>`

The opening tag is `<p>` and the closing tag is `</p>`.

The `/` tells the browser that the element is ending.

## Elements We Covered

### Headings

HTML has six heading levels:

- `<h1>` - largest / most important heading
- `<h2>`
- `<h3>`
- `<h4>`
- `<h5>`
- `<h6>` - smallest / least important heading

Example:

`<h1>My Name is Devon</h1>`

The heading numbers are not only about size. They also help organize the structure and importance of the content on a page.

### Paragraph

`<p>` is used for normal paragraph text.

Example:

`<p>I am learning HTML at CodeCrew.</p>`

### Links

The `<a>` element is called an **anchor tag** and is used to create links.

The destination of the link is usually placed inside an attribute such as `href`.

### Buttons

The `<button>` element creates a button.

Example:

`<button>Click Me</button>`

HTML can create the button itself, while other technologies like JavaScript can later control what happens when the button is clicked.

### Images

The `<img>` element displays an image.

Example:

`<img src="images/devon.jpeg" alt="Photo of Me" width="300">`

Some important image attributes:

- `src` - tells the browser where the image file is
- `alt` - alternative text describing the image for accessibility or if the image cannot load
- `width` - controls the displayed width of the image

I also learned that file paths matter. If my image is inside an `images` folder, I can use:

`src="images/devon.jpeg"`

## Attributes

Attributes give additional information or settings to an HTML element.

They are written inside the opening tag.

Example:

`<img src="images/devon.jpeg" alt="Photo of Me">`

Some attributes we discussed:

- `id` - gives one specific element a unique identifier
- `class` - allows multiple elements to share the same identifier/group
- `name` - often used to identify data, especially in forms
- `src` - specifies a source file
- `href` - specifies where a link goes

## VS Code

VS Code can help write HTML using **IntelliSense/autocomplete**.

It can suggest tags and automatically complete some code, but I still need to understand what it is adding and make sure my opening and closing tags are in the correct places.

## What I Practiced

For today's first lab, I created an **About Me webpage from scratch**.

I:

- Created a new GitHub repository
- Cloned the repository to my computer
- Created an `index.html` file
- Created an `images` folder
- Added my name using a heading
- Added my age using a heading
- Added a picture using an `<img>` element
- Added a short description using a `<p>` element
- Changed the browser tab title with `<title>`
- Used the `width` attribute to resize my image
- Committed my changes
- Pushed the project to GitHub
- Submitted my repository link for the assignment

## Something That Clicked for Me

HTML is basically the **structure of the webpage**. It tells the browser what the different pieces of content are.

For example, instead of the browser only seeing some text, HTML can tell it:

- this is a heading
- this is a paragraph
- this is an image
- this is a link
- this is a button

Later, CSS can control how those things look, and JavaScript can control more of how they behave.

---

## Day 3 - Part 2: Structuring a Page

### Images - Width, Height, and Alt Text

We went over images again and learned more about controlling their size.

The `<img>` element can use `width` and `height` attributes to control how large the image appears.

Example:

```html
<img src="images/photo.jpg" width="300" height="300" alt="Photo description">
```

We also reviewed the `alt` attribute.

`alt` gives the image a text description. This is important for accessibility, especially for screen readers, and can also provide information if the image does not load.

I also learned that the order of attributes inside an opening tag does not matter. For example, `src`, `width`, `height`, and `alt` can be arranged in different orders and the browser will still understand them.

Pixel measurements are written with `px` when using CSS, such as:

```html
style="width: 300px;"
```

## Ordered Lists

The `<ol>` element creates an **ordered list**.

An ordered list normally displays its items using numbers.

Each item inside the list uses an `<li>` element.

Example:

```html
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

- `<ol>` = ordered list
- `<li>` = list item

The `<li>` elements need to be placed inside the `<ol>`.

## Parent and Child Elements

We learned that HTML elements can exist inside other HTML elements.

When one element contains another element:

- The outside element is the **parent**
- The element inside it is the **child**

Example:

```html
<ol>
    <li>First item</li>
</ol>
```

In this example:

- `<ol>` is the parent
- `<li>` is the child

This is called **nesting**.

## Unordered Lists

The `<ul>` element creates an **unordered list**.

It works similarly to an ordered list, but it normally displays bullet points instead of numbers.

Example:

```html
<ul>
    <li>Music</li>
    <li>Coding</li>
    <li>Gaming</li>
</ul>
```

The difference is:

- `<ol>` = numbered list
- `<ul>` = bulleted list
- `<li>` = an item inside either type of list

I can also add text before a list to explain or describe what the list contains.

Example:

```html
<p>My Favorite Things:</p>

<ul>
    <li>Music</li>
    <li>Coding</li>
    <li>Gaming</li>
</ul>
```

## Tables

The `<table>` element is used to organize information into rows and columns.

Some of the table elements we learned are:

- `<table>` - contains the entire table
- `<tr>` - table row
- `<th>` - table header cell
- `<td>` - table data cell
- `<thead>` - groups the heading section of a table
- `<tbody>` - groups the main data section of a table

Example:

```html
<table>
    <tr>
        <th>Movie</th>
        <th>Year</th>
        <th>Trailer</th>
    </tr>

    <tr>
        <td>Movie Name</td>
        <td>2026</td>
        <td>Trailer Link</td>
    </tr>
</table>
```

A `<tr>` represents one horizontal row.

Inside the row:

- `<th>` is used for headings
- `<td>` contains the actual data

This is another example of parent and child relationships because the cells are nested inside rows, and the rows are nested inside the table.

## Links Inside Tables

For the lab, I learned how to place an anchor tag inside a table data element.

Example:

```html
<td>
    <a href="https://www.youtube.com/">Trailer</a>
</td>
```

The `<td>` creates the table cell.

The `<a>` element inside it creates the clickable link.

The `href` attribute tells the browser where the link should go, while the text between `<a>` and `</a>` is what appears on the webpage.

## `<link>` vs `<a>`

I also learned that `<link>` and `<a>` are different HTML elements.

### `<link>`

The `<link>` element is normally placed inside the `<head>`.

It connects the webpage to outside resources, such as a CSS stylesheet, and works behind the scenes.

Example:

```html
<link rel="stylesheet" href="styles.css">
```

### `<a>`

The `<a>` element is used inside the `<body>` to create a visible and clickable link.

Example:

```html
<a href="https://www.youtube.com/">YouTube</a>
```

A simple way to remember this is:

- `<link>` = connects resources to the webpage
- `<a>` = creates a link that the user can click

## Semantic HTML

We were introduced to **semantic HTML**.

Semantic HTML means using elements that describe the meaning or purpose of the content they contain.

This helps make webpages:

- Easier for developers to understand
- Better organized
- More accessible
- Easier for search engines to understand

Instead of HTML only describing how something should appear, semantic elements can also describe what that content represents.

## Wireframing

Before building a webpage, it can help to create a **wireframe**.

A wireframe is a simple visual plan for the structure of a webpage before writing the actual code.

It can show things like:

- Headers
- Navigation
- Main content areas
- Sections
- Images
- Buttons
- Menus
- Spacing

The purpose is to think about the layout and organization first before worrying about the finished design.

## Browser DevTools

Browser DevTools can be used to inspect the HTML behind a webpage.

The **Elements** tab lets me see how the webpage is structured and how different elements are nested.

Shortcuts:

- `F12`
- Windows: `Ctrl + Shift + I`
- Mac: `Cmd + Shift + J`

This can be useful for understanding how existing websites are built and for debugging my own HTML.

## What I Practiced

For the second lab, I created another HTML project from scratch.

I practiced:

- Creating a second GitHub repository
- Creating an `index.html` file
- Using a table to organize information
- Creating rows with `<tr>`
- Adding data with `<td>`
- Adding links inside table cells
- Using `<a>` and `href` to link to movie trailers
- Making sure elements were properly opened and closed
- Understanding how nested elements create parent/child relationships
- Committing and pushing the finished project to GitHub

## What I Learned Today

The biggest thing I learned today is that HTML is not just about putting things onto a webpage. The way elements are **structured and nested** matters.

A webpage is made up of elements inside other elements, and each element has a specific purpose.

For example:

- A list contains list items
- A table contains rows
- Rows contain table cells
- A table cell can contain a link

Learning the parent/child relationship makes it easier to understand how larger webpages are organized.