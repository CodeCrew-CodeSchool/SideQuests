# Week 01 Day 02 - CSS Styling Methods

## What I Learned Today

Today I learned the three main ways to add CSS to an HTML page:

- Inline CSS
- Internal CSS
- External CSS

I also practiced using classes, styling a `<div>`, changing colors, and centering content on a webpage.

## Inline CSS

Inline CSS is written directly inside an HTML element using the `style` attribute.

Example:

```html
<div style="background-color: skyblue; color: yellow; text-align: center;">
```

Multiple CSS properties can be added inside the same `style` attribute and are separated with semicolons.

Inline CSS is useful when styling one specific element, but it could get difficult to manage if a page had a lot of styling.

## Internal CSS

Internal CSS is written inside a `<style>` element, usually inside the `<head>` of the HTML document.

Example:

```html
<style>
    .rocket-div {
        background-color: midnightblue;
        color: silver;
        text-align: center;
    }
</style>
```

The styles can then be connected to an HTML element by giving that element a class.

```html
<div class="rocket-div">
```

## CSS Classes

A class lets me create a group of styles and apply them to an HTML element.

In CSS, a period (`.`) before a name means I am targeting a class.

```css
.rocket-div {
}
```

This connects to:

```html
<div class="rocket-div">
```

The name `rocket-div` is not a built-in CSS command. It is just the name of the class. The CSS class name and the HTML `class` value need to match.

## External CSS

External CSS keeps the CSS in a separate `.css` file instead of putting it directly inside the HTML file.

The HTML page connects to the CSS file using a `<link>` element inside the `<head>`.

Example:

```html
<link rel="stylesheet" href="styles.css">
```

Then the CSS rules can be written inside something like:

```text
styles.css
```

External CSS is useful because it keeps the HTML structure and CSS styling more organized and separate.

## Inline CSS vs Inline Elements

One thing I want to remember is that inline CSS and inline HTML elements are different things.

**Inline CSS** means CSS is written directly inside an HTML element using `style=""`.

**Inline elements** describe how certain HTML elements behave on the page.

For example, `<span>` and `<img>` are normally inline elements, while `<div>` is normally a block element.

## Centering Content

I learned that:

```css
text-align: center;
```

does more than just center text.

It centers inline content inside the element too. Since an `<img>` behaves like an inline element by default, using `text-align: center;` on its parent `<div>` also centered the rocket image.

## Today's Lab

For today's lab, I created a page for a Space Rocket toy and practiced two different CSS methods.

### Part 1

I used inline CSS to:

- Change the background to sky blue
- Change the text to yellow
- Center the heading
- Center the rocket image

### Part 2

I recreated the page using an internal `<style>` element and a class called `rocket-div`.

I used:

```css
.rocket-div
```

to select the class and:

```html
class="rocket-div"
```

to apply the styles to the `<div>`.

## Reminders for Later

- CSS controls the appearance of HTML.
- Inline CSS uses `style=""`.
- Internal CSS uses a `<style>` element.
- External CSS uses a separate `.css` file.
- A `.` before a selector means it is a class.
- The class name in CSS must match the class name in HTML.
- CSS properties inside a rule end with semicolons.
- `text-align: center;` can center inline content such as text and images.