## About Testing in WordPress Playground
Testing in WordPress Playground is a way to ensure that your code is working as expected. It is a crucial part of the development process, as it helps to identify bugs and issues early on, before they reach production. 

There are different types of testing that can be done in the Playground, including unit testing, integration testing, end-to-end testing, and performance testing. 

This document provides an overview of the different types of testing that can be done in the Playground, as well as some best practices for testing your code. 

###  Integration Testing - // needs docs, what is, tests

###  [End-to-End](../e2e-testing-in-playground.md) Testing
-  Testing with [PHPUnit](./testing-PHPUnit.md)
-  Testing with Playwright - link to [Gutenberg packages](https://github.com/WordPress/gutenberg/tree/trunk/packages/e2e-test-utils-playwright)

## Testing with Cypress
Cypress is a popular testing framework for web applications. It is a fast, easy-to-use tool that allows you to write and run tests for your web applications.
-  E2E Tests with Cypress - [#802](https://github.com/WordPress/wordpress-playground/pull/802)


# Testing Plugins

## Enable Live Previews on WordPress.org/plugins
You can enable a live demo of your plugin on WordPress.org/plugins by following the steps outlined in Enabling [Plugin Previews](../plugin-previews.md).

## Testing a plugin
[Walkthrough testing a plugin](./testing-a-plugin.md) with the VS Code Extension

## Testing a theme
Import [theme unit test data](./import-theme-unit-test-data.md) to test your theme. Some current limitations bust mostly working.

The following URL will showcase the TwentyTwentyFour theme with the theme unit test data imported.

https://playground.wordpress.net/?php=8.0&wp=6.4&storage=none&networking=yes&import-content=https://raw.githubusercontent.com/WordPress/theme-test-data/master/themeunittestdata.wordpress.xml


Tracking testing coverage
-  E2E Test Coverage - Tracking - [#807](https://github.com/WordPress/wordpress-playground/issues/807)

### Misc testing
-  Testing with Selenium
-  Testing with [Jest](./testing-with-jest.md)
-  Performance Testing

---


## Accessibility Testing
Learn more [about accessibility testing](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/accessibility/) in WordPress
Accessibility testing considerations

[a11y-theme-unit-test](https://github.com/wpaccessibility/a11y-theme-unit-test)


### Considerations
Are you testing the Playground itself or a website created with the Playground?
- more info here: [#612](https://github.com/WordPress/wordpress-playground/issues/612)
- If you test Playground itself, make sure it's a brand new instance by resetting and deleting the files you were working on.
- For safety purpose it's recommend not to do a hard-delete via the command-line or keyboard shortcuts, but rather to drag the folder to the trash. 
- If you are absolutely sure you don't want these files anymore, you can delete them permanently.

 (this is not) testing accessibility in Playground, make sure you are testing against the instance and not the website created in the instance

## Roadmap
Unit Testing with PHPUnit - [blocked by #1250](https://github.com/WordPress/wordpress-playground/pull/1250)

E2E tests for GitHub integration [#805](https://github.com/WordPress/wordpress-playground/issues/805)

E2E tests for the local filesystem sync [#806](https://github.com/WordPress/wordpress-playground/issues/806)

[WordPress Coding Standards WPCS](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/) - using with the Playground