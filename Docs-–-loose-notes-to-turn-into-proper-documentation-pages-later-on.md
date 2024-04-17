## Various questions and discussions

* [How to self-host Playground, load Blueprints, embed it in WP?](https://wordpress.slack.com/archives/C04EWKGDJ0K/p1711536092257959) 
* [How to load older WordPress releases?](https://github.com/WordPress/wordpress-playground/issues/994#issuecomment-2027158712)

## How to debug wasm?

* Existing docs
* https://github.com/vshymanskyy/awesome-wasm-tools/blob/main/README.md
* https://github.com/WordPress/wordpress-playground/issues/1128
* https://github.com/WordPress/wordpress-playground/issues/1078
* https://github.com/WordPress/wordpress-playground/issues/134
* Check these WASM PRs and the related discussions:
    * https://github.com/WordPress/wordpress-playground/pull/993
    * https://github.com/WordPress/wordpress-playground/pull/1115
    * https://github.com/WordPress/wordpress-playground/pull/1114
    * https://github.com/WordPress/wordpress-playground/pull/1104
    * https://github.com/WordPress/wordpress-playground/issues/354

---

## How do I detect if my code is running in Playground?

From https://github.com/WordPress/wordpress-playground/issues/483:

I recommend **not** detecting Playground because it will break your plugin in many contexts.

You could, however, explicitly create a constant via a Blueprint and test for that:

https://playground.wordpress.net/#{%22constants%22:{%20%22MYPLUGIN_SETUP_DEMO_CONTENT%22:%22true%22}}

This way your plugin will only load the demo data when that's expected.

I understand why blanket Playground detection is tempting for setting up demo content. Playground, however, is more than just the app on https://playground.wordpress.net/. Here's a few contexts where loading the demo content would be harmful instead of useful:

* The [WordPress Playground plugin](https://github.com/WordPress/playground-tools/releases/tag/v0.1.65) adds a "Preview now" button to the plugin directory. It imports the entire sites and installs the plugin on top of that. 
* [wp-now](https://www.npmjs.com/package/@wp-now/wp-now) is a local development environment for WordPress. Your plugin may be installed there.
* Ditto for [WordPress Playground for VS Code](https://marketplace.visualstudio.com/items?itemName=WordPressPlayground.wordpress-playground).

If installing the plugin does something unexpected to the site content in either of these tools, the user will likely be surprised and assume the plugin is broken.

Any Playground-specific variable or constant is a private API and may get renamed or disappear without a warning. A long-term goal for Playground is to have 1:1 feature parity with native PHP and be indistinguishable from it.

More content:

* https://github.com/WordPress/wordpress-playground/issues/483#issuecomment-2009360012
* https://github.com/WordPress/wordpress-playground/issues/483#issuecomment-2009408222
