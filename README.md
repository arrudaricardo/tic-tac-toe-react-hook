# React Hooks Tic-Tac-Toe

## Introduction
React Hooks is a new addition to [React version 16.8](https://reactjs.org/docs/hooks-intro.html
), allowing to use State in Function. I personally prefer to work with Function over Class in Javascript and now we can do it.
The Idea for this Tutorial is to reproduce the game [Tic-Tac-Toe](https://en.wikipedia.org/wiki/Tic-tac-toe
) using React Hooks.

## Setup
For this tutorial we going to user [ create-react-app ](https://github.com/facebook/create-react-app
), so be sure to have [ Nodejs and NPM](https://nodejs.org/en/
) install in your computer.


In your terminal execute the command:
```````bash
npx create-react-app tic-tac-toe
cd tic-tac-toe
````````
Now that we create a React App open the directory with a text editor of your choice e.g [VIM](https://www.vim.org/
)

## Create Components 

All your source files will be inde de src/ directory. Lets create a new directory for our components.

Inside tic-tac-toe/src create a new /components directory and two new files **Table.js** and **TicBlock.js**.
The Table.js going to be a component that going to wrap the TicBlock.js, Ticblock.js are going to be each of the 9 blocks that the user can add X or O.

We need to import Table to our App.js first.

App.js
```
import React from 'react';
// Allow us to use JXS
import './App.css';
// Import the Style
import Table from './components/Table'
// Import the Table.js components
function App() {
  return (
      <div>
          <Table />
       </div>
  );
}


export default App;
//export in order to be imported by index.js, that is the root file for this App.
```
If you need more information about the JSX please check this [Link](https://reactjs.org/docs/introducing-jsx.html
).

Know we can edit the **Table.js** component.
First we need to import the Hook [ userState ](https://reactjs.org/docs/hooks-reference.html#usestate
) and [ useEffect ](https://reactjs.org/docs/hooks-reference.html#useeffecthttps://reactjs.org/docs/hooks-reference.html#useeffect
). Hooks *are functions that let you “hook into” React state and lifecycle features from function components*[^1]
[^1]: https://reactjs.org/docs/introducing-jsx.html


