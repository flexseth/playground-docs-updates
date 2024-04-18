This document is a work in progress. Want to contribute examples?
Please do! 

## How to boot up Playground in easy mode
`wp-content` mode 
- Loads up everything in the `wp-content` directory
- Themes, Plugins, and Uploads

This is a great option if you want to create a new theme for a website. 
Or want to work with an existing website to test out a plugin or theme.

You have all of the content, import the existing website content, and can now work on re-theming the site.

### How to boot up Playground in `wp-content` mode
1. Find what you want to work on and open the `wp-content` directory
2. In VS Code, it's important that the project bar at the top reads `wp-content`
   - This is how you can tell you're in the right directory
3. Click "Start WordPress Server" to instantiate the WordPress server
4. If using `wp-now` from the command-line, use...
 - `npx @wp-now/wp-now start` - from the `wp-content` directory

When you close out your terminal or VS Code the `wp-now` process will stop your web server.

In order to get back into the same Playground, you'll simply want to restart Playground from the same folder location. There may be a port change but the site will have your changes saved.

## Contents
WordPress installation should include the following:
- All uploaded media to this website
- The current theme being used
- All plugins being used



