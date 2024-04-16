## About the Theme Unit Test Data collection
WordPress theme unit test data is a collection of test data for WordPress themes. It is used to test the compatibility of themes with WordPress. The data includes posts, pages, comments, custom post types, tags, categories, and more.

It showcases the style of the elements, and creates pages with examples of almost every type of content you can create in WordPress. The purpose is to check to see how the theme handles each of these different types of content, with various layouts, and if style adjustments are needed. It is a way to provide a visual check-out of an entire website, one of the steps to making the website fully production ready. 

## Import Theme Unit Test Data in Playground
You can import the theme unit test data into a WordPress Playground instance to test the compatibility of themes with WordPress. The theme unit test data can be imported using the WordPress importer plugin.
The following URL will showcase the TwentyTwentyFour theme with the theme unit test data imported.

This technique uses the Query API for Playground approach to append the necessary parameters to the end of the Playground Online's [URL](https://playground.wordpress.net)

https://playground.wordpress.net/?php=8.0&wp=6.4&storage=none&networking=yes&import-content=https://raw.githubusercontent.com/WordPress/theme-test-data/master/themeunittestdata.wordpress.xml

---

## Needs CORs headers 
Something isn't working, but I didn't track it down.
https://github.com/WordPress/wordpress-playground/issues/718

### Possible workaround
- It is a CORS issue (simply include in URL fragment?)
- Or convert to another API example (ie. `fetch`)

