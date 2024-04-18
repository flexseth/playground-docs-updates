## Known Limitations
- Shell steps don't work in `wp-now` - [#1166](https://github.com/WordPress/wordpress-playground/issues/1166)


## Known Issues
See the [WordPress Playground](https://github.com/WordPress/playground-tools/labels/wp-now) for all known issues.

-   Running `wp-now start` in 'wp-content' or 'wordpress' mode will produce some empty directories: [WordPress/wordpress-playground#328](https://github.com/WordPress/wordpress-playground/issues/328)
-   Inline images are broken when site starts on a different port: [WordPress/wordpress-playground#356](https://github.com/WordPress/wordpress-playground/issues/356)
-   `wp-now` doesn't build or start on Windows: [WordPress/playground-tools#66](https://github.com/WordPress/playground-tools/issues/66), [WordPress/playground-tools#11](https://github.com/WordPress/playground-tools/issues/11)
-   It's not possible to set `WP_DEBUG` and other `wp-config.php` constants: [WordPress/playground-tools#17](https://github.com/WordPress/playground-tools/issues/17)
-   In 'wordpress' mode, `wp-now` can connect to a MySQL database with `define( 'DB_HOST', '127.0.0.1' );`, but `define( 'DB_HOST', 'localhost' );` does not work: [WordPress/wordpress-playground#369](https://github.com/WordPress/wordpress-playground/issues/369)
-   `wp-now` published versions can appear random: [WordPress/wordpress-playground#357](https://github.com/WordPress/wordpress-playground/issues/357)

### Importing and exporting
- Playground Plugin: Can't import via .sql file - [#1124](https://github.com/WordPress/wordpress-playground/issues/1201)
  - Blocked by needing Passwordless login 