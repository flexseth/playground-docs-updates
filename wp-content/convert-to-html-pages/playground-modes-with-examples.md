## Automatic Modes
Understanding the context in which you are working on the Playground while doing local development.

## How you can boot Playground
Using `wp-now` or the VS Code Extension, you can boot Playground in a couple of different ways. The main difference is, it depends on what project folder (for VS Code extension), or directory (for `wp-now`) you are working in.

`wp-now` automatically operates in a few different modes for both the start and the php commands. Here's [more info](./about-wp-now.md) on `wp-now` modes:

The selected mode depends on the directory in which it is executed:

- Plugin Mode
- Theme Mode
- Content Mode - load up wp-content

Loads the project files into a virtual filesytem with WordPress and a SQLite-based database. Everything (including WordPress core files, the database, wp-config.php, etc.) is stored in the user's home directory and loaded into the virtual filesystem. The latest version of WordPress will be used, unless the `--wp=<version>` argument is provided. 

[**Examples**](#)

---

## Plugin mode
Presence of a PHP file with 'Plugin Name:' in its contents.

Here's an example for using Plugin Mode

[**Examples**](#)

---

## Theme mode 
The basic ingredient for a Theme is the presence of a `style.css` file with an updated `'Theme Name:'` in the theme header.

```PHP
/*
Theme Name: Block Theme
Description: Built with Playground
...
*/

```

To create a brand new block theme, you will need the `Create Block Theme` plugin actiated, let's take a look at how to to do that. 

[**Examples**](#)
How to build a [block theme](./creating-themes-with-playground.md) based on TwentyTwentyFour with Playground
- [ ] Showcase step-by-step demo
- [ ] Showcase a blueprint with a block theme

---

## wp-content mode

Presence of plugins and themes subdirectories.
Here's an example for using content mode

wordpress: Runs the directory as a WordPress installation when WordPress files are detected. An existing wp-config.php file will be used if it exists; if it doesn't exist, it will be created along with a SQLite database.

**Examples**
`wp-content` mode 
- Loads up everything in the `wp-content` directory
- Themes, Plugins, and Uploads

This is a great option if you want to create a new theme for a website. 

Or want to work with an existing website to test out a plugin or theme.

### How to boot up Playground in `wp-content` mode
`wp-content` mode is helpful if you are working on an existing website or41
1. Find what you want to work on and open the `wp-content` directory
2. Click "Start WordPress Server" to instantiate the WordPress server
3. If using `wp-now` from the command-line, use...
 - [ ] TODO: Instructions for doing this with `wp-now`
 - [ ] TODO: Walkthrough for the workflow

## Contents
WordPress installation should include the following:
- All uploaded media to this website
- The current theme being used
- All plugins being used


---

## WordPress Develop mode
Same as wordpress mode, except the build directory is served as the web root.

Documentation needed for this mode.

[**Examples**](#)

---

## index.php mode
When an index.php file is present, starts a PHP webserver in the working directory and simply passes requests to the index.php.
playground: If no other conditions are matched, launches a completely virtualized WordPress site.

[**Examples**](#)

