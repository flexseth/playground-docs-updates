## Ideas
Understanding dependencies in the Playground

Dependency management is an important part of plugin development.
Developers need to be aware of what dependencies are needed for their plugin to work correctly. 

> Developers using @wordpress/scripts to build their assets need to manually include the `wp-polyfill` dependency if they need polyfills.

### Scope
- Explain what `wp-polyfill` is, and why it would be needed as a dependency
- Show how to create a blueprint to create a basic plugin with the `wp-polfill` dependency
- Showcases working with webpack and dependency management in the Playground

## What is `wp-polyfill`
`wp-polyfill` is a package that provides polyfills for modern JavaScript features that are not supported in older browsers.

### How does `wp-polyfill` work
First by detecting if the user is running a modern browser. 
Then, if it's necessary to "polyfill" - add some scripts for support to older browsers.

Let's say you are working on a JavaScript Carousel that provides support with WordPress's `wp-polyfill`.

If you don't include the `wp-polyfill` dependency, the carousel will not work in older browsers.