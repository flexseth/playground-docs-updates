## About `wp-now`
> wp-now streamlines the process of setting up a local WordPress environment.
See the NPM package on [wp-now](https://www.npmjs.com/package/@wp-now/wp-now).

See [more info](about-wp-now-more-info.md) to dive deeper, learn about boot modes and more.

## Requirements
`wp-now` includes an entire WordPress environment, so you don't need to install WordPress separately. It runs on PHP WASM.

`Node.js` is required to run `wp-now`. You can download it from the [Node.js website](https://nodejs.org/).
Node is required because the Playground using NPM under the scenes to install packages.

---

## Automatic boot modes
Review [more info about](about-wp-now-more-info.md) `wp-now`
And [Playground Modes with examples](playground-modes-with-examples.md) for more information on how to boot up Playground.


## Allowing Plugin Previews on WordPress.org
Add blueprint.json file to enable plugin previews #481
- https://github.com/WordPress/create-block-theme/issues/481

## Limitations
The `shell` step currently won't work in `wp-now` because it doesn't support the `shell` command.
This is a known limitation that we are working towards making work! 
- [ ] TODO: Clarify what common "shell" type things you can do another way in `wp-now`

Please check the Playground Tools GitHub repo for [issues related to](https://github.com/search?q=repo%3AWordPress%2Fwordpress-playground+wp-now&type=issues) `wp-now` 

---

## Security warnings
Sometimes when you use packages from an external source, the project you are using needs to update them. 

See the [Security Warnings](./playground-tools/wp-now/fixing-security-warnings.md) page for more information on how to audit and fix security issues in `wp-now`.

You can report these types of errors if you aren't able to get them fixed.
Here is a sample error report on the `playground-tools` repo
- [wp-now: Resolve npm audit warnings #224](https://github.com/WordPress/playground-tools/issues/224)
- [ ] TODO: Update docs with how to audit and fix security issues in `wp-now`


> wp-now: Error starting: getaddrinfo ENOTFOUND
- https://github.com/adamziel/playground-docs-workflow/issues/32


## Updating `wp-now` docs on the Playground Tools repo
Documentation for using wp-now with Playground [#31](
https://github.com/adamziel/playground-docs-workflow/issues/31)