
## Week10_Learnings - 3-10-01 - Blog 

**Learning points (chronological order)**

- HTTP: Acronym for Hypertext Transfer Protocol - Protocol that enables your web browser to communicate with a web server to load webpages

- API: Acronym for Application Programming Interface - Set of defined rules and specifications that allows different software applications to communicate and interact with each other. It acts as an intermediary, enabling one program to request services or data from another program, without needing to know the intricate details of how the other program is built or operates.

- **Request Response Cycle**
1. User Action: User does something — like clicking a link, submitting a form, or typing a URL
2. Browser Sends Request: Browser packages that action into an HTTP request and sends it to the web server
3. Server Receives Request: Server reads the request and figures out what resource or data the browser is asking for
4. Server Processes Request: Server responds to the ask - might fetch a file, run some code, query a database, or dynamically generate a response 
5. Server Sends Response: Server sends back an HTTP response — often an HTML page, JSON data, or an error message
6. Browser Receives Response: Browser interprets the data, renders the web page (or updates part of it), and displays it to the user


***Diagrams - simple and more complex https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Server-side/First_steps/Client-Server_overview***



- **HTTP requests** 

A message sent from a client (like a browser) to a server asking for data or to perform an action (e.g., view a page or submit a form). The action includes details like the method (GET, POST, etc.), the URL, and sometimes extra information (like headers or form data). Two example follow - each starting with CAP letters.

GET /index.html HTTP/1.1 → asks the server to send back the web page index.html. POST /login HTTP/1.1 → sends form data (like username and password) to the server to process a login.

- **API fetch** 

A JavaScript function that sends an HTTP request from code — often to get or send data from an API instead of loading a full webpage.

API returns a Promise, which lets the script handle the server’s response (e.g., converting it to JSON and displaying it on the page).


- **API integration into webpage with HTML and JavaScript**

Overview of what API integration means and how it appears in a simple webpage:

🌐 API Integration (1–3 Bullets)

- An API integration connects a webpage to outside data or services — like weather info, maps, or news — using JavaScript to send and receive information.

- The webpage’s HTML provides a place to show the results (like a <p> or <div>), while JavaScript handles the request and updates the page.

- This makes a webpage dynamic — it can display live or personalized data instead of static text.

💡 Common Real-World Example: A visitor checks the current weather for their city — the page calls a weather API and displays live temperature and conditions.

🧩 Simple Example Syntax - HTML, then JS

**HTML (display area and button)**

<button onclick="getWeather()">Show Weather</button>
<p id="weather"></p>


**JavaScript (fetching data from an example API, and catch in case of problems)**

function getWeather() {
  fetch('https://api.example.com/weather?city=Memphis')
    .then(response => response.json())
    .then(data => {
      document.getElementById('weather').innerHTML = 
        "Temperature: " + data.temp + "°C";
    })
    .catch(error => console.log("Error:", error));
}


***If something breaks (like no internet), the catch block handles it gently instead of crashing the page.***


**CRUD** 
CRUD is a core concept in web development and database work, and it ties directly into what you’ve been learning about APIs, HTTP requests, and webpage interactions.

CRUD stands for the four basic actions that software (and APIs) perform on data:

| **Letter** | **Action** | **Plain Meaning**                  | **Common HTTP Method** | **Example (Web Context)**                                  |
|------------|------------|------------------------------------|------------------------|------------------------------------------------------------|
|    **C**   | **Create** | Add new data to a database or API. | `POST`                 | A visitor fills out a sign-up form to create an account.   |
|    **R**   | **Read**   | Retrieve or view existing data.    | `GET`                  | A webpage loads user profiles or weather info from an API. |
|    **U**   | **Update** | Modify existing data.              | `PUT` or `PATCH`       | A user edits their profile picture or updates a comment.   |
|    **D**   | **Delete** | Remove existing data.              | `DELETE`               | A user deletes a saved post or cancels a booking.          |
