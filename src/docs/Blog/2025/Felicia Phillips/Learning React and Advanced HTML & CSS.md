### ⭐ Learning React

React is a frontend JavaScript library used for building users interfaces, particularly for single-page applications. It is a tool for building UI components. 

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

