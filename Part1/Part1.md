# Part1

## Initialize
```bash
npm create vite@latest introdemo --template react
```

Run the template by the following commands:
```bash
cd introdemo
npm install
npm run dev
```

## Make soem changes
Edit to simplify the main.jsx and App.jsx files in the `src` directory.
```js
import ReactDOM from 'react-dom/client'

import App from './App'

ReactDOM.createRoot(document.getElementById('root')).render(<App />)
```

```js
const App = () => {
  return (
    <div>
      <p>Hello world</p>
    </div>
  )
}

export default App
```

The file App.jsx now defines a [React component](https://react.dev/learn/your-first-component) with the name App. The command on the final line of file main.jsx
> React lets you combine your markup, CSS, and JavaScript into custom “components”, reusable UI elements for your app. 

index.html contains the HTML code that is used to render the React application. The file is located in the `public` directory, and it contains a `<div>` element with the id `root`. This is where the React application will be rendered.

main.jsx is the entry point of the React application. It imports the ReactDOM library and the App component, and it renders the App component into the `<div>` element with the id `root` in index.html.