# DEVELOPER DOUBTS AND PRACTICES

Yo mysterysolver here learning and building things.Here I have noted down ideas,concepts,commands that I usually want to look back.

## what is node.js?

It is a RTE(run time environment). It is sued to run js servers outside a server for web building. Express is a framework built on top of node.js.
This is a middleware which makes life simpler in routing and other stuff.If we are not importing anything there is no need for node package manger to play a role.

## what is npm?

npm is node package manager.which is used to manage dependecy,versions in package.json.This makes easy development and installation.

## what is npx?

npx is node package executor.This installs everything in local cache without corrupting the global one.Also this uses the latest version.
This doesn't fuss over global paths and stuff.

## what is react?

It is a component based reac library. 
It uses virtual DOM.In vanilla js we manage our DOM elements but in vite ot manages.Vanilla js is imperative proggraming paradigm.React is declarative pp.
Imperative involes telling computer each and every step what to do and how to do.This is similar to vanilla js.Here we handle the real dom by us and our code whihc is slower.
[React Vs Vannilla Js](https://medium.com/@mattidungafa/react-vs-vanilla-js-an-imperative-vs-declarative-story-8a5eedbff212)
It is hard to manage each and every component on a scalable system.In declarative pp,we define what should happen for a UI state and react does the rest.
Learning involves writing JSX instead of core js.System manages they state.

<br>

we can export components here.
return jsx(js XML) which is the UI component.
React updates only the changed part efficently than doing fully chnage.

## what is vite?

It is developed by Evan yu. vite means fast.He majorly used ES modules.
ESMAScript is the standard system for sharing and packaging js code.wkt ES6 of 2015 has this import and export features.
It is asynchronous in nature and it's with the type="module".

## Imports in React

Make sure all the export,imports,filename is the same.Filename should be same if it is a default import. If it is a named import we would use the const keyword. For default imports don't use {}.Because curly braces is used for named imports.

## React work space

```
function myComponent(){
  //space to handle logics,hoooks,event listener and helper methods.
  return (
      //here we return JSX UI!
)
}
```

## .forEach and .map

forEach doesn't return values and map returns the array it traverses.Thus we can't use it inside the curl braces where it should return JSX.
Those curly braces are js expression containers ahm.

## sending data across routes in react

[How to pass and access data from one route to another with useLocation, useNavigate, useHistory hooks.](https://dev.to/esedev/how-to-pass-and-access-data-from-one-route-to-another-with-uselocation-usenavigate-usehistory-hooks-1g5m).
we are using useNavigate,useLocation,useHistory,state propert to transfer data.


