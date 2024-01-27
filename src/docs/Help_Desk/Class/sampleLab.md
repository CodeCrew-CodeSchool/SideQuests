# Lab: T-Shirt Sales
Read this lab assignment in its entirety before beginning your lab. You may want to open it in a new tab.

## Problem Domain
Your friend Alex has a new business idea of selling unique t-shirts inspired by famous artworks. Alex has a collection of t-shirt designs featuring various art pieces and wants to create an application to manage the sales projections and inventory for each design.

Alex needs your assistance in building a proof of concept application that can calculate the number of t-shirts to produce daily based on certain factors such as operating hours, customer traffic, and average t-shirts sold per customer. This will help Alex manage inventory and production schedules effectively.

In addition to those backend calculations, Alex also wants you to design a public-facing webpage to showcase the t-shirt collection, provide information about each design, and display sales projections for each design.

## Instructions
To get started, accept your assignment from Github Classroom and Clone this repo to your local machine.

Create two new pages within your project: "Sales Data" (sales.html) and the homepage (index.html). You'll also need to create a JavaScript file, for example, app.js.

### Sales Data
In your JavaScript file, create separate objects for each t-shirt design. Each design will have its own sales data calculations and display on the webpage. You should be able to perform the following tasks:

In object properties, store:
* the minimum and maximum hourly customers, 
* and the average t-shirts sold per customer

Use a method of each object to generate a random number of customers per hour.
[Objects/Math/random](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random)

Calculate and store the projected number of t-shirts sold for each hour for each design.

Display the projected sales for each design as an unordered list on the webpage.

Calculate the total projected sales for each design and display it.

Your output for each design should look like this:

Artwork A
- 10am: 15 t-shirts
- 11am: 20 t-shirts
- 12pm: 25 t-shirts
- ...
- 6pm: 12 t-shirts
- Total: 140 t-shirts
Display the lists on sales.html.

Home Page
Your index.html file should include the following:

A custom font from [Google Font](https://fonts.google.com/) for headings.

Specified standard web fonts for different text types.
Different font colors for headings and text.
Background colors for the default page background and elements like boxes and tables.
A layout that is organized and easy to navigate.
Information about the t-shirt collection, designs, and the business.
Contact information, hours of operation, and other relevant details.


Developer Style Guide
Ensure that your project follows these guidelines:

Create a new branch for each day's work (e.g., day1-features).

Include .gitignore and .eslintrc.json files.

Commit regularly within your non-main branches.

Use meaningful names for properties, methods, and functions.

Follow the single-responsibility principle.

Utilize template literals for rendering data on the webpage.

Stretch Goals
Create low-fidelity and high-fidelity wireframes for your webpage based on the provided articles.

Implement responsive design to ensure your webpage looks good on various devices.

Resources
Refer to the Setting up a new project{:target="_blank"} document for initial project configuration.
Submission Instructions
Submit the link to your GitHub repo for this project.
Deploy your GitHub repo using GitHub Pages{:target="_blank"}. Submit the link to your deployed site.
Answer the following questions in the Canvas submission:
How did this assignment go, overall?
What observations or questions do you have about what you've learned so far?
How long did it take you to complete this 