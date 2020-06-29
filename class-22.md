# Props
Components accept arbitrary inputs called `props`. In JSX, props are passed into a component with a syntax that looks like HTML attributes. These are the equivalent of function params.

In actuality, `props` is the name of the object passed into a component constructor and any prop added to a component in the JSX will be accessible as a property on `props`.

After `props` is passed into the constructors `super` function, they are available on the context by using this.`props`.

Props Example … the way we get to use them
```
const element = (
  <h1 className="greeting">
    Hello, world!
  </h1>
);
```


[Home Page](https://osamamousa204.github.io/reading-notes-401/)
