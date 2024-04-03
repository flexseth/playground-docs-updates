## Introduction
Code for Ryan Welcher’s live stream Thursday, April 4, 2024

## WIP
Some steps are incomplete or incorrect on purpose.

The goal is to work through this in real time, to show how the Playground works, and to demonstrate how to test a plugin in the Playground.

- [Download the VS Code Extension for WordPress Playground](https://marketplace.visualstudio.com/items?itemName=WordPressPlayground.wordpress-playground)
- Open a New Window in VS Code
- Activate the plugin in VS Code
- Create a new directory, `working-with-plugins-in-playground`  and enter

```bash
mkdir ~/Desktop/working-with-plugins-in-playground && cd $_ && code .
```

- Close the original window, make sure you’re working in the
    - `working-with-plugins-in-playground` directory
    - **insert screenshot**
    
    []()
    
- Clone the repo so you can test out a block
    - `gh repo clone WordPress/block-development-examples`
- Enter the directory and search for a plugin you want to work on
    - `cd block-development-examples/plugins`
- Let’s try out the Interactivity API Countdown block
    - `cd interactivity-api-countdown-3cd73e`
- Start WordPress Server - click me!
    - This will launch Playground in **Plugin** mode so you can demo this block
    - **GOTCHA!** Wrong folder
        - Stop WordPress Server
- **FIX:** Open a new VS Code window from this directory
    - `code .`
- Close out the old window for simplicity
    - Now click Start WordPress Server
        - You should see a fresh install with the Interactivity API Countdown block available
        - Your block is installed **and activated!**
- Insert the block to test it on a post
    - **Show how to do this programmatically**

## An easier way…

Find the block files, get into that folder as your root project folder, **Launch WordPress Server**

---

## Takeaways…

- Block doesn’t work without a build step - how to build?
    - Where are the files to build?
    - `wp-scripts` not found…
        - `npm i`
- Block still doesn’t work..
    - Must install interactivity api dependency
- Improvements are coming to this flow
- Good for testing
- Git workflows?
- Does data persist?
- How to destroy?
- How to stop from running?
- Is it building? How to build…
    - Accessing the local filesystem…
    - etc