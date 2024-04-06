## Automatic Modes
`wp-now` automatically operates in a few different modes for both the start and the php commands. 

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
Presence of a style.css file with 'Theme Name:' in its contents.
Here's an example for using Theme Mode

[**Examples**](#)

---

## wp-content mode
Presence of plugins and themes subdirectories.
Here's an example for using content mode

wordpress: Runs the directory as a WordPress installation when WordPress files are detected. An existing wp-config.php file will be used if it exists; if it doesn't exist, it will be created along with a SQLite database.

[**Examples**](#)

---

## WordPress Develop mode
Same as wordpress mode, except the build directory is served as the web root.

[**Examples**](#)

---

## index.php mode
When an index.php file is present, starts a PHP webserver in the working directory and simply passes requests to the index.php.
playground: If no other conditions are matched, launches a completely virtualized WordPress site.

[**Examples**](#)