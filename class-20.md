# Component based UI systems 
* React
* Angular
* Vue

### React
As a component based system, React does an awful lot for us, principally, it gets out out of the way and makes it EASY to implement your application the way you see it, using familiar tools.

**jsx**
Why JSX?
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.
```
const element = () => {
  return {
    <h1 className="greeting">
      Hello, world!
    </h1>
  }
);
```
Behind the scenes…
```
const element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);
```
##### react examble
```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```




[Home Page](https://osamamousa204.github.io/reading-notes-401/)
