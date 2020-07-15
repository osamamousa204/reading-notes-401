# Managing the Redux Store

### Different Practices

- File and Directory Names
- Reducer and Action Styles
- How do we model our data in the reducers

## Redux ToolKit

#### This toolkit specifies a few different means of building a reducer and action set that work well together and are easier to understand and integrate

Ultimately, your store code can be as simple and declarative as this:


```
const postsSlice = createSlice({
name: ‘posts’,
initialState: [],
reducers: { createPost(state, action) {},
updatePost(state, action) {},
deletePost(state, action) {} } })
```
## Resources:
- https://redux-toolkit.js.org/
- https://github.com/erikras/ducks-modular-redux
[Home Page](https://osamamousa204.github.io/reading-notes-401/)
