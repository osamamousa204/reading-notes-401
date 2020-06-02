# router.param(name, callback)

Adds callback triggers to route parameters, where name is the name of the parameter and callback is the callback function. Although name is technically optional, using this method without it is deprecated starting with Express v4.11.0 (see below).

The parameters of the callback function are:

req, the request object.
res, the response object.
next, indicating the next middleware function.
The value of the name parameter.
The name of the parameter.

## Middleware

Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

### Types of Middleware
Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.

- validate
- save
- remove
- updateOne
- deleteOne
- init (note: init hooks are synchronous)


**Query middleware is supported for the following Model and Query functions. In query middleware functions, this refers to the query** 

- count
- deleteMany
- deleteOne
- find
- findOne
- findOneAndDelete
- findOneAndRemove
- findOneAndUpdate
- remove
- update
- updateOne
- updateMany

### Subdocuments

Subdocuments are documents embedded in other documents. In Mongoose, this means you can nest schemas in other schemas. Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.
### What is a Subdocument?

Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.

[Home Page](https://osamamousa204.github.io/reading-notes-401/)