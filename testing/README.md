## About Testing in WordPress Playground
Testing in WordPress Playground is a way to ensure that your code is working as expected. It is a crucial part of the development process, as it helps to identify bugs and issues early on, before they reach production. 

There are different types of testing that can be done in the Playground, including unit testing, integration testing, end-to-end testing, and performance testing. 

This document provides an overview of the different types of testing that can be done in the Playground, as well as some best practices for testing your code. 
-  Integration Testing
-  End-to-End Testing - [#805](https://github.com/WordPress/wordpress-playground/issues/805)
-  Testing with Playwright
-  Testing with Cypress
-  Testing with Selenium
-  Testing with [Jest](./testing-with-jest.md)
-  Performance Testing

## Testing with Cypress
Cypress is a popular testing framework for web applications. It is a fast, easy-to-use tool that allows you to write and run tests for your web applications.

[Testing with Cypress - #802](https://github.com/WordPress/wordpress-playground/pull/802) 

## Testing a plugin
[Walkthrough testing a plugin](./testing-a-plugin.md) with the VS Code Extension

## Testing a theme
Import [theme unit test data](./import-theme-unit-test-data.md) to test your theme. Some current limitations bust mostly working.

The following URL will showcase the TwentyTwentyFour theme with the theme unit test data imported.

https://playground.wordpress.net/?php=8.0&wp=6.4&storage=none&networking=yes&import-content=https://raw.githubusercontent.com/WordPress/theme-test-data/master/themeunittestdata.wordpress.xml



## Accessibility Testing
Accessibility testing considerations
- Are you testing the Playground itself or a website created with the Playground?
- more info here: [#612](https://github.com/WordPress/wordpress-playground/issues/612)
- If you test Playground itself, make sure it's a brand new instance by resetting and deleting the files you were working on.
- For safety purpose it's recommend not to do a hard-delete via the command-line or keyboard shortcuts, but rather to drag the folder to the trash. 
- If you are absolutely sure you don't want these files anymore, you can delete them permanently.

 (this is not) testing accessibility in Playground, make sure you are testing against the instance and not the website created in the instance

## Roadmap
Unit Testing with PHPUnit - [blocked by #1250](https://github.com/WordPress/wordpress-playground/pull/1250)

E2E tests for GitHub integration [#805](https://github.com/WordPress/wordpress-playground/issues/805)
