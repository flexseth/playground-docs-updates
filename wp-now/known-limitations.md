## Common errors
> command not found: wp-now

You must install `wp-now`, please visit the `NPM` [package page](https://www.npmjs.com/package/@wp-now/wp-now#known-issues) to install.

## Known Limitations
These issues were pulled from the Playground Tools and WordPress Playground repositories. 

## Known Issues
See the [WordPress Playground](https://github.com/WordPress/playground-tools/labels/wp-now) for all known issues. `wp-now` is a great tool and we look forward to hearing your feedback, stress testing the project, and improving it over time.


## `wp-cli`
Very limited support for `wp-cli` outside of use with blueprints
- WP-NOW: Add wp-cli integration [#212](https://github.com/WordPress/playground-tools/pull/212)
- `Shell` steps don't work in `wp-now` - [#1166](https://github.com/WordPress/wordpress-playground/issues/1166)


#### Boot modes
Quirky boot modes
`wp-now` recognizes the context you are booting in, which can have some quirky behavior.

- Replace "Mode" concept with auto-loading or explicit CLI flags [#26](https://github.com/WordPress/playground-tools/issues/26)
- Data carrying-over between instances in VS Code extension - "Playground" mode [#1184](https://github.com/WordPress/wordpress-playground/issues/1184)
- Running `wp-now start` in 'wp-content' or 'wordpress' mode will produce some empty directories: [WordPress/wordpress-playground#328](https://github.com/WordPress/wordpress-playground/issues/328)
- wp-now: don't expect a full wp-content directory in wp-content mode [#244](https://github.com/WordPress/playground-tools/issues/244)

#### Plugins and Themes
`installPlugin` and `installTheme` steps
- wp-now: blueprint with installPlugin steps fails on subsequent runs [#209](https://github.com/WordPress/playground-tools/issues/209)

`Must Use Plugins`
- `wp-now` doesn't support custom `mu-plugins` [#73](https://github.com/WordPress/playground-tools/issues/73)
- What is the best way to load my mu-plugins? [#198](https://github.com/WordPress/playground-tools/issues/198)
- mu-plugin folder not loaded when using pre-existing install [#101](https://github.com/WordPress/playground-tools/issues/101)
- wp-now detects wp-content mode if there is a mu-plugins subdir inside the dir where it is executed. [#234](https://github.com/WordPress/playground-tools/issues/234)
- The theme directory "twentytwentyfour" does not exist. [#1240](https://github.com/WordPress/wordpress-playground/issues/1240)


#### Database and file systems
- wp-now: Allow mounting host filesystem [#245](https://github.com/WordPress/playground-tools/issues/245)
- WordPress crashes when connecting to MySQL [#237](https://github.com/WordPress/playground-tools/issues/237)
- wp-now: Error establishing database connection when 'DB_HOST' is 'localhost' [#18](https://github.com/WordPress/playground-tools/issues/18)
- Local Environment: Workflow to import an existing MySQL database [#15](https://github.com/WordPress/playground-tools/issues/15)
- Allow a configuration to map other folders and files [#19](https://github.com/WordPress/playground-tools/issues/19)
- wp-now: crashes when trying to access wp-admin with a remote database [#1052](https://github.com/WordPress/wordpress-playground/issues/1052)
- .wp-now/mu-plugins/sqlite-database-integration-main/db.copy: Not a directory or a symbolic link to a directory [#230](https://github.com/WordPress/playground-tools/issues/230)
  - Must install the sqlite-database-integration plugin


#### Routing
-   Inline images are broken when site starts on a different port: [WordPress/wordpress-playground#356](https://github.com/WordPress/wordpress-playground/issues/356)
-   In 'wordpress' mode, `wp-now` can connect to a MySQL database with `define( 'DB_HOST', '127.0.0.1' );`, but `define( 'DB_HOST', 'localhost' );` does not work: [WordPress/wordpress-playground#369](https://github.com/WordPress/wordpress-playground/issues/369)
- SSL: Local Environment: Support SSL connections [#24](https://github.com/WordPress/playground-tools/issues/24)
- wp-now: Error starting: getaddrinfo ENOTFOUND [#32](https://github.com/adamziel/playground-docs-workflow/issues/32)

#### Windows
-   `wp-now` doesn't build or start on Windows: [WordPress/playground-tools#66](https://github.com/WordPress/playground-tools/issues/66), [WordPress/playground-tools#11](https://github.com/WordPress/playground-tools/issues/11)
- VS Code Extension: Windows 10 and PHP versions lower than 8.0 [#13](https://github.com/WordPress/playground-tools/issues/13)
- Compatibility with Windows and WSL [#435](https://github.com/WordPress/wordpress-playground/issues/435)

#### Debugging
- wp-now: Constant WP_DEBUG already defined [#135](https://github.com/WordPress/playground-tools/issues/135)
-   It's not possible to set `WP_DEBUG` and other `wp-config.php` constants: [WordPress/playground-tools#17](https://github.com/WordPress/playground-tools/issues/17)
-   `wp-now` published versions can appear random: [WordPress/wordpress-playground#357](https://github.com/WordPress/wordpress-playground/issues/357)
- Support Xdebug [#314](https://github.com/WordPress/wordpress-playground/issues/314)

### Blueprint steps
- `wp-now` does not activate plugins or themes via activatePlugin and activateTheme step. [#241](https://github.com/WordPress/playground-tools/issues/241)


### Importing and exporting - Migrations
- Playground Plugin: Can't import via .sql file - [#1124](https://github.com/WordPress/wordpress-playground/issues/1201)
  - Blocked by needing Passwordless login 
- Image links broken when moving from wordpress-playground to wp-now [#942](https://github.com/WordPress/wordpress-playground/issues/942)
- CORS header workaround needed for Theme Unit Test import [#718](https://github.com/WordPress/wordpress-playground/issues/718)
- Plugins on `SVN` won't properly import test data (see [#99](https://github.com/WordPress/blueprints-library/issues/99))

#### Performance
- wp-now: out of memory error when running for many hours [#96](https://github.com/WordPress/playground-tools/issues/96)
- wp-now only runs a single PHP process which means PHP cannot issue a HTTP request to itself. [#239](https://github.com/WordPress/playground-tools/issues/239)