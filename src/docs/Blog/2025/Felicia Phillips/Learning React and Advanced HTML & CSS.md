## ⭐ Learning React
React is a frontend JavaScript library used for building users interfaces, particularly for single-page applications. It is a tool for building UI components. 

React is a declarative system where you provide a state that you want the system to create without worrying about the DOM manipulations needed to change what's displayed in the browser. 

## Create React App
**Run this command to create a React application named my-react-app:**
```javascript
npx create-react-app my-react-app
```

## Run the React Application
**Run this command to move to the my-react-app directory** 
```javascript
cd my-react-app
```

**Run this command to execute the React application my-react-app**
```javascript
npm start
```
A new browser window will pop up with your newly created React App! If not, open your browser and type localhost:3000 in the address bar.

### Upgrading an existing React application
Step 1: Install React 18 
To install the latest version, from your project folder run the following from the terminal:
```javascript 
npm i react@latest react-dom@latest
```
Step 2: 
Use the new root API
```javascript 
import ReactDOM from 'react-dom/client';
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<App />);
```
## How does React Work ?

- It creates a virtual dom in memory. 
- Instead of manipulating the browser's DOM directly, React creates a virtual DOM in memory, where it does all the necessary manipulating, before making the changes in the browser DOM.
- React finds out what changes have been made, and changes only what needs to be changed.


## Building React UI

 ### 1. Break up the UI into a component hierarchy. (Split it up into reusable components)
 ### 2.  Build Static Version in React
  - Create Separate .js or .jsx Files for each component. For example: <code> Header.js (or Header.jsx) Sidebar.js (or Sidebar.jsx) </code>
  - Within each file, define a React component that returns the static JSX structure. <br>
  example:
  ```javascript
  function SearchBox() {
  return (
    <div>
      <input type="text" placeholder="Search Google or type a URL"/>
    </div>
  );
}
export default SearchBox;
  ```
  - Wrap All Components in App() on App.js
   Example:
```javascript
import React from 'react';
import Header from './Header';
import SearchBox from './SearchBox';

function App() {
  return (
    <div>
      <Header />
      <SearchBox />
      {/* ... other components */}
    </div>
  );
}

export default App;
```
### 3. Identify the state
 - Determine what data should cause the user interface to change.
 - **The data that causes the user interface to change is called state**
### 4. Identify where the state should live.
- Figure out which component should hold the state (the component that needs to modify or pass down the data).
### 5. Add inverse data flow by using events and event handlers.
- Parent components pass down event handler functions as props to child components.
- Child components call these handler functions when events occur, passing data back to the parent.
- This allows child components to trigger state changes in their parents, leading to UI updates.

