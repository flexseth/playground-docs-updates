## Must-use Plugins
These types of plugins are required for a website to function correctly.

### What are Must-use Plugins?
Must-use plugins are plugins that are automatically activated on a WordPress site. They are also known as mu-plugins. These plugins are stored in the `wp-content/mu-plugins` directory and are automatically activated when WordPress is loaded. Must-use plugins are useful for adding functionality to a site that should not be disabled by the user.

 ### `mu-plugins` vs `Requires Plugins` header
 In the context of the Playground, `mu-plugins` are typically a piece of code that runs when a blueprint is executed.

 `mu-plugins` can be used to
 
 #### Customize the WordPress environment (`options`)
 - Customize permalinks - see [example blueprint](./options-set-permalinks.json)
 - Set the site title - see [example blueprint](./options-set-site-title.json)
 - Create values in the `wp-config.php` file - see [example blueprint](./options-set-wp-config-values.json)
 
 #### Interact with posts and pages
 - Create pages and posts - see [example blueprint](./create-post.json)
 Notice for WordPress's built-in functionality to work, the `wp-load` function must be called first