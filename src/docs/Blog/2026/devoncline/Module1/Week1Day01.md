# Week 01 - Day 01 - Introduction to CSS

## What is CSS?

Today we started learning **CSS (Cascading Style Sheets)**.

HTML is mainly responsible for the **structure and content** of a webpage, while CSS controls how that content **looks**.

For example:

- HTML creates a heading.
- CSS can change its color, size, font, position, spacing, and more.

A basic CSS rule follows this pattern:

```css
selector {
    property: value;
}
```

Example:

```css
h1 {
    text-align: center;
}
```

- `h1` = selector
- `text-align` = property
- `center` = value

The selector tells CSS **what element to target**, the property tells it **what to change**, and the value tells it **how to change it**.

---

## Styling HTML Elements

CSS can target different HTML elements individually.

Example:

```css
h1 {
    color: blue;
}
```

This changes the text color of all `<h1>` elements.

Styles can also be applied directly to an HTML element:

```html
<h1 style="text-align: center;">My Heading</h1>
```

The `style` attribute allows CSS to be written directly inside an HTML element.

For now, we are mainly practicing CSS this way before separating CSS into its own file.

---

## Styling the Body

The `<body>` contains most of the visible content on a webpage.

Because other elements are located inside the body, it is useful for setting styles that should apply across most of the page.

Example:

```css
body {
    font-family: Arial;
    color: black;
    background-color: white;
}
```

Setting a font on the body usually causes text inside of it to use that font unless another element has its own font specified.

For example:

```css
body {
    font-family: Arial;
}

h1 {
    font-family: Georgia;
}
```

Most of the page would use Arial, but the `<h1>` would use Georgia instead.

---

## The CSS Box Model

CSS treats HTML elements like boxes.

The main parts of the box model are:

1. **Content** - The actual text, image, or other content.
2. **Padding** - Space between the content and its border.
3. **Border** - The line or edge around the element.
4. **Margin** - Space outside the element separating it from other elements.

A simple way to remember it:

**Content → Padding → Border → Margin**

Example:

```css
img {
    padding: 10px;
    border: 2px solid black;
    margin: 20px;
}
```

### Padding

Padding adds space **inside** an element.

```css
padding: 10px;
```

### Border

Borders create a visible edge around an element.

```css
border: 2px solid black;
```

Borders can have different styles, thicknesses, and colors.

### Margin

Margins create space **outside** an element.

```css
margin: 20px;
```

Margins are useful for controlling the distance between elements.

---

## Border Radius

`border-radius` rounds the corners of an element.

Example:

```css
border-radius: 10px;
```

It can be used on things such as:

- Images
- Buttons
- Cards
- Containers
- Profile pictures

A large border radius or `50%` can sometimes make a square image appear circular.

```css
border-radius: 50%;
```

Border radius is mostly a **design choice**. It is not something every element needs.

---

## Fonts

The `font-family` property changes the typeface used for text.

Example:

```css
font-family: 'Courier New', Courier, monospace;
```

This is a list of possible fonts the browser can use.

The browser tries them from left to right:

1. `Courier New`
2. `Courier`
3. Any available `monospace` font

A **monospace font** gives every character the same amount of horizontal space.

Monospace fonts are commonly associated with programming, code editors, and terminals.

---

## CSS Files

CSS can eventually be stored in a separate file, commonly named:

```text
style.css
```

The HTML file can connect to it using:

```html
<link rel="stylesheet" href="style.css">
```

Keeping CSS in a separate file is useful because multiple HTML pages can use the same styles.

For today's assignment, we practiced putting styles directly on HTML elements instead.

---

## Line Breaks in HTML

Typing blank lines inside a `<p>` element does not automatically create visible blank lines in the browser.

The `<br>` element creates a line break.

Example:

```html
First line<br>
Second line
```

Two line breaks can create additional spacing:

```html
<br><br>
```

This was useful for keeping the different sections of the poem separated.

---

## Lab - Poem Page

For today's lab, I created a webpage displaying a poem and its author.

The assignment required:

- A header containing the poem title
- A header containing the author's name
- A paragraph containing the poem
- The title centered using CSS
- The author centered using CSS
- A different font applied to the poem

I used:

```css
text-align: center;
```

to center the title and author.

I used:

```css
font-family: 'Courier New', Courier, monospace;
```

to change the font of the poem.

The poem I chose was **"All Watched Over by Machines of Loving Grace" by Richard Brautigan**, which describes a future involving computers, humans, and nature.

---

## Main Things to Remember

- HTML creates the structure of a webpage.
- CSS controls how the webpage looks.
- CSS follows `selector { property: value; }`.
- Padding is space inside an element.
- Margin is space outside an element.
- Borders surround elements.
- `border-radius` rounds corners.
- `font-family` changes fonts.
- Styles placed on a parent element can affect elements inside of it.
- CSS can be written directly in HTML or stored in a separate `.css` file.