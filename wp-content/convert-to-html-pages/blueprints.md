Welcome to Blueprints for the WordPress Playgound 
## All about blueprints
Common use cases, configurations, one-click demos of WordPress in the browser.

---

### What are blueprints?
Blueprints define a series of steps to take when installing WordPress. 

Written in `JSON` format, steps can do anything WordPress can do and more. 

[Blueprints](#) can be used to [install plugins](https://wordpress.github.io/wordpress-playground/blueprints-api/steps#InstallPluginStep), [themes](https://wordpress.github.io/wordpress-playground/blueprints-api/steps#InstallThemeStep), and [configure settings](https://wordpress.github.io/wordpress-playground/blueprints-api/steps/#SetSiteOptionsStep). Blueprints can be used to [automate processes](#), [import websites](#), and for [testing purposes](#).

Presenting the opportunity to revolutionize the way we work with WordPress.


[Here's a list of what all is possible with blueprints](https://wordpress.github.io/wordpress-playground/blueprints-api/)
- [ ] Update doc for "everything you can do with Playground"
- https://github.com/WordPress/wordpress-playground/issues/1094

---

## How to run blueprints?
Blueprints are used to configure a website at **initial setup**, not to modify an existing website. If you want to destroy your beautiful sandcastle, read more about [resetting Playground environments.](./RESET-PLAYGROUND.md)  

Currently, blueprints can be only used

---

### Functionality and limitations

Essentially, most anything you can do in WordPress or PHP can be automated via a blueprint. If you find a limitation or a feature you'd like to see, please open up an issue in the [Playground Tools](https://github.com/WordPress/playground-tools/issues) repo. 

When reporting issues please use the various issue starter templates!

Blueprints API is in [V1](https://wordpress.github.io/wordpress-playground/blueprints-api/), which is written in TypeScript. Work is in progress to create a new version that will be written in PHP.

---

## How to use Blueprints?
There are a couple of ways to test blueprints: 
- Go to the blueprint previewer
- [Use `wp-now`](./wp-now.md) to run your blueprint locally
- Copy/paste your blueprint into the playground.net URL bar

---

## Gotchas!
Blueprints are meant to be run on a fresh WordPress environment. If you have already run a blueprint on the same environment, you will need to reset the environment before running the blueprint again.

In `wp-now`, you can reset the environment by running `wp-now --reset`

**Note:** This will delete all the data in the environment. Use carefully.

---

## Blueprint tools
Blueprint schema is probably the most important tool for building blueprints. It defines the structure of the blueprint and the available options. The schema is used to validate the blueprint and provide a user-friendly interface for creating blueprints.


Including the [blueprint schema](./examples/blueprint-schema.json) at the top of your blueprint will give access to code completion and validation in your code editor.

---

### `wp-now`
`wp-now` is a command-line tool that allows you to run blueprints locally. It is a great way to test your blueprints before running them in the WordPress Playground. The package serves as a standalone WordPress installation with some idiosyncracies...

Learn more about `wp-now` 


---

## Migrations
Migrations are a way to move a WordPress website from one server to another. This can be for demonstration purposes, testing, or to move a website from a local environment to a live server.

Please see the [Migrations docs](./migrating.md) for more info


##### Migration methods
- import from a  [WXR file](https://wordpress.github.io/wordpress-playground/blueprints-api/steps#ImportWxrStep) (WordPress eXtended RSS - an XML file format)
- import from [WP-CLI](https://github.com/WordPress/blueprints-library/issues/90)
- migrate [database and files](./wp-content/html-pages/migrate-database-and-files.md)


---

## Resources
- [Blueprints onboarding documentation #64](https://github.com/WordPress/blueprints-library/issues/64)
- [Blueprints API](https://wordpress.github.io/wordpress-playground/blueprints-api/)

---

## Examples
[See blueprint examples](./EXAMPLES.md)
[Working with blueprint options](./OPTIONS.md)
[Blueprint Previewer](https://wordpress.github.io/wordpress-playground/blueprint-previewer/)
[Create a blueprint from a website](#)

---


## Using the filesystem
This was auto generated. Needs improvement

Playground files are found in the `/home/user/.wp-now` directory. This directory is mounted to the `/var/www/html` directory in the WordPress container. This means that you can access the files in the Playground by navigating to `/var/www/html` in the WordPress container.


---

## Playground Tools for Blueprints
- VS Code extension - best for basic testing and plugin development
- Data persistence between Playground instances as described [here]()

---

## Testing in Playground
- [Testing a plugin in Playground](playground/testing-a-plugin.md)  

---

## Known limitations
- Blueprints do not work with `wp-now` or the VS Code extension
- Sometimes it's necessary to open a new window and copy/paste your blueprint URL into the URL bar to run it
- GitHub caches pages and is tough to cache bust - blueprint files may not update immediately
- Formatting and sharing blueprints can be difficult, here's a tool for that 

---

###### TODO
## Features requested
Check out the [roadmap](./roadmap.md) for more information on what's coming up next.

Everything listed in the [Blueprints library issue](https://github.com/WordPress/blueprints-library/issues/64)


#### Links to add and address
[Tracking: Redesign Documentation](https://github.com/WordPress/wordpress-playground/issues/217)

### How to: 
- [ ] Showcase my plugin or theme (live demos on .org)
- [ ] Control the embedded website
- [ ] provide interactive code snippets
- [ ] preview pull requests from my repo
- [ ] development environment without Apache or MySQL: `wp-now` vs. [VS Code Extension](./playground-tools/vs-code-extension.md)
- [ ] Contributing to the Playground