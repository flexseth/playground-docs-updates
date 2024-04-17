

## Pull Request Previewer Online
A product made to modernize the request review process for WordPress. It is a web-based tool that allows users to preview pull requests from GitHub repositories. The tool is designed to be used by developers, designers, and other contributors to the WordPress project.

## System Requirements: None
We are working hard to make sure that all users can utilize the PR Previewer online interface, regardless of the device or operating system they are using. The PR Previewer online is a web-based tool that can be accessed from any device with an internet connection and a web browser.

## How to use the PR Previewer Online
Using the PRROP - Pull Request Reviewer Online Previewer

To use the PR Previewer, follow these steps
1. Someone sends you a link to a PR to review
2. Click on the link to open the PR Previewer
3. Optionally compare the PR to another one, by opening a new browser

Streamlining the progress of getting changes to everyone. 
The PR previewer is essentially a snapshot at a point in time of the software lifecycle.

## How to Integrate the PR Previewer with your project
Playground offers a built-in functionality for creating previews directly from pull requests. This functionality is utilized in the wordpress-develop repository's workflow (https://make.wordpress.org/core/handbook/contribute/git/github-pull-requests-for-code-review/). A CI action comments on every Pull Request with a Playground preview link:
    
    ```markdown
    [Preview on Playground](https://playground.wordpress.net/?pr=12345)
    ```     

## More info
How to add Pull Request previews to your repository? [#1237](https://github.com/WordPress/wordpress-playground/issues/1237)


