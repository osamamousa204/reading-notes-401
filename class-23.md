# Component Composition

### Routing
Using `react-router`, you can easily toggle the visibility of components (or even pages) based on the URL/Route that the user engages with.

`import { Route } from 'react-router-dom';`

To use Browser Router properly, you eliminate your use of `<a>` tags and instead use it’s built-in `<Link>` component.
```
<Link to="/">Home</Link>
<Link to="/stuff">Stuff</Link>
```

In practice, then, use the router component to look at either / or /stuff and based on that, displaying either the Home or the List component…

```
<Route exact path="/" component={Home} />
<Route exact path="/stuff" render={() => <List>{items}</List>} />
```

#### React’s props.children

The React docs say that you can use props.children on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’. For me, that didn’t really clear things up. I’m sure for some, that definition makes perfect sense but it didn’t for me.
My simple explanation of what this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

[Home Page](https://osamamousa204.github.io/reading-notes-401/)
