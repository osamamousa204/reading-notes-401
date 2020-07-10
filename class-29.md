# Getting Started with Redux
Redux is a predictable state container for JavaScript apps.

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger.

You can use Redux together with React, or with any other view library. It is tiny (2kB, including dependencies), but has a large ecosystem of addons available.

### Installation
Redux is available as a package on NPM for use with a module bundler or in a Node application:
```
# NPM
npm install redux

# Yarn
yarn add redux
```
It is also available as a precompiled UMD package that defines a window.Redux global variable. The UMD package can be used as a `<script>` tag directly.

For more details, see the Installation page.

# Redux Toolkit
Redux itself is small and unopinionated. We also have a separate addon package called Redux Toolkit, which includes some opinionated defaults that help you use Redux more effectively. It's our official recommended approach for writing Redux logic.

RTK includes utilities that help simplify many common use cases, including store setup, creating reducers and writing immutable update logic, and even creating entire "slices" of state at once.

Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

# Create a React Redux App

The recommended way to start new apps with React and Redux is by using the official Redux+JS template for Create React App, which takes advantage of Redux Toolkit and React Redux's integration with React components.

Copy

```
npx create-react-app my-app --template redux
```

[Home Page](https://osamamousa204.github.io/reading-notes-401/)
