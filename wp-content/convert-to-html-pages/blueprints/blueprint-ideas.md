## Proof of concepts for Blueprints
Support for [10 Initial Blueprints](https://github.com/adamziel/blueprints/issues/1) for the Community Gallery

Here are a list of ideas of what you could conceivably do with Blueprints.

### Blueprint Ideas

#### Design & Development
- Create a new custom block
 - scaffold a new block via the `create-block` package
 - include steps for build setup
 - uses CLI input to bring variables to create block ingredients
- `create-block-theme` 
- `create-block-plugin` 
 - scaffold a plugin via `WP-CLI`
 - or try using the [Better Plugin Boilerplate](https://github.com/TukuToi/better-wp-plugin-boilerplate)
- Generate content using Fakerpress (plugin demo, content)
- Block Library - create a block library
 - a blueprint that creates a block library
 - or create an interface to create multiple blocks

#### Testing
- Theme Unit Test - must fix [Add CORS headers]
- WordPress Coding Standards (`WPCS`) - install Plugin Review Check and run on a plugin
- Theme Check - install `Theme Check` [plugin](https://wordpress.org/plugins/theme-check/) and run on a theme

#### Demos, Sharing, Collaboration, Teaching
- Demo a plugin with a blueprint that imports relevant content
- Share a blueprint with a colleague
- Collaborate on a Playground with a colleague
 - create a new user account via `wp-cli` 
 - share access (export/import)
- Teach a class how to build a plugin
 - use `create-plugin` utility
 - install Playground Plugin
 - open a page with an `Interactive Code` block on it

### Deep Linking
Stylebook
- add custom styles to theme.json via the CLI
- or define your custom styles in the root directory, write to `theme.json` file
- Jump to the stylebook to view the custom styles

### Maintenance
Start with a "completely fresh" WordPress install
- Remove all extra pages and all content (start completely fresh)

### Blueprint utilities
Automatically add CORS support if needed
- CORS - automatically add CORS support if needed to support the blueprint
- scan blueprint for need, if so, add CORS support

Automatic networking detection
- Network detection is turned off by default
- scan blueprint for need, if so, turn on networking

Keywording
- Add keywords to the blueprint for searchability
- scan the blueprint for keywords common to the `plugins` directory
- add keywords to the blueprint `metadata`
