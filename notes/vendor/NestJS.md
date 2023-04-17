# Nest JS

## Core

### Controllers

Controllers are responsible for handling incoming requests and returning responses to the client.

### Providers

The main idea of a provider is that it can be injected as a dependency; this means objects can create various relationships with each other, and the function of "wiring up" instances of objects can largely be delegated to the Nest runtime system.

### Modules

Each application has at least one module, a root module. The root module is the starting point Nest uses to build the application graph - the internal data structure Nest uses to resolve module and provider relationships and dependencies.

### Middleware

Middleware is a function which is called before the route handler. 

### Exception filters

When an exception is not handled by your application code, it is caught by this layer, which then automatically sends an appropriate user-friendly response.

### Pipes

Pipes have two typical use cases:

- transformation: transform input data to the desired form (e.g., from string to integer)
- validation: evaluate input data and if valid, simply pass it through unchanged; otherwise, throw an exception

### Guards

Guards have a single responsibility. They determine whether a given request will be handled by the route handler or not, depending on certain conditions (like permissions, roles, ACLs, etc.) present at run-time. This is often referred to as authorization. 

### Interceptors

They make it possible to:

- bind extra logic before / after method execution
- transform the result returned from a function
- transform the exception thrown from a function
- extend the basic function behavior
- completely override a function depending on specific conditions (e.g., for caching purposes)

### Custom decorators

Nest provides a set of useful param decorators that you can use together with the HTTP route handlers.


## Courses

- [Official NestJS Courses](https://courses.nestjs.com/)
