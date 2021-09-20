# React - Dev Setup and Deployment

This assignment is intented to help you set up your development environment for React. You will create a simple React App and deploy using one of the methods covered in lecture.

## Step 1
- Install `npx` following the instructions here: https://www.npmjs.com/package/npx
- run `npx create-react-app my-first-app` to create the React application
- In the newly created app, replace the contents of `App.js` including your name:

```
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <p>Hello CSCI E-39!</p>
        <p>
          My name is ____________
        </p>
      </header>
    </div>
  );
}

export default App;
```

- run `npm install`
- start the app with `npm start`
- verify the app is running
- modify line 6 in `App.test.js` to:

`const linkElement = screen.getByText(/Hello CSCI E-39!/i);`

- make sure all tests pass when running `npm run test` 

## Step 2
Deploy the application using one of the methods covered in class: Github Pages, Render, or AWS. If you prefer to use a different service, explain your choice and process.

## Submitting
Edit this file (README.md) and complete the following:

- URL to live application: https://reem2411.github.io/sample-react/
- How did you deploy it? 
    - After creating my repo on github and pushing my static files to github through github desktop, I followed the follownig steps from the react deployment code README file: 
    commit your files (make sure package-lock.json is there)
      - In package.json, add a new key/value as: "homepage": "https://<user>.github.io/<repo>"
      - In Github, Go to Settings -> Pages -> in Source -> gh-pages branch -> Click Save
      - Once the build-deploy action finishes running, the app should be live at https://<user>.github.io/<repo>
- What code editor are you using? VSCode 

That is all!
