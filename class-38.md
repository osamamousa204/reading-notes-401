# Redux - Asynchronous Actions

## Async Actions
Three different kinds of actions:
- An action informing the reducers that the request began:
  - The reducers may handle this action by toggling an isFetching flag in the state. This way the UI knows it's time to show a spinner.
- An action informing the reducers that the request finished successfully:
  - The reducers may handle this action by merging the new data into the state they manage and resetting isFetching. The UI would hide the spinner, and display the fetched data.
- An action informing the reducers that the request failed:
  - The reducers may handle this action by resetting isFetching. Additionally, some reducers may want to store the error message so the UI can display it.


## Using Redux actions to connect to **remote APIs** via Thunk Middleware

Action generators **return a function**:
```
const get = (payload) => {
  return {
    type: 'GET',
    payload: payload
  }
}
```
- Must perform asynchronous action before dispatching to reducer.

- The action you dispatch from your **React App** returns a function.

- Not an actual action object, which is what Redux expects and requires.

```
let api = 'https://api.mockable.io/api/v1/stuff';

export const get = () => dispatch => {
  return utils.fetchData(api).then(records => {
    dispatch(getAction(records));
  });
};

const getAction = payload => {
  return {
    type: 'GET',
    payload: payload,
  };
};
```
- Implement redux middleware: `“thunk”`

- **Inspects** every dispatched action


## Asynchronous Redux Actions Using Redux Thunk
#### Installation & Setup
```
$ yarn add redux-thunk

# or, using npm:
$ npm install redux-thunk
```

#### Basic Usage:
1. retrieve or save data
1. easy to dispatch actions that follow the lifecycle of a request to an external API
