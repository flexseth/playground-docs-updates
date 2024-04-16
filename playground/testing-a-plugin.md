## Testing Plugins (in VS Code) with Playground
A working walkthrough of testing a plugin in Playground. It involves the current process to work with a Playground instance in VS Code. 

Please contribute to this document by submitting a PR to the docs repo. Using feature branches is recommended, but not required. If you find something broken, please open an issue.

The repo is made to represent a problem and solution case, where you can walk through the steps to see how to build a plugin in the Playground. We are going to use the `Block Development Examples` repo to test a block in the Playground.


## WIP
Some steps are incomplete or incorrect on purpose.

By the end it would be nice to have a functioning walkthrough with how to solve any problems that come up along the way of testing plugins. 

## Testing a Plugin in Playground
The goal is to work through this in real time, to show how the Playground works, and to demonstrate how to test a plugin in the Playground.

Make sure you have the VS Code Extension installed and enabled
- [Download the VS Code Extension](https://marketplace.visualstudio.com/items?itemName=WordPressPlayground.wordpress-playground)
- Open a New Window in VS Code      // Docs needed, screen flows
- Activate the plugin in VS Code    // Docs needed, screen flows
- Create a new directory, `working-with-plugins-in-playground`  and enter
- Once installed, you will see a new button in the toolbar and also in the command palette
    - **insert screenshot** // Docs needed, screen shot
- If you click the WordPress toolbar button, you will be taken to a pretty simple UI for now
    - **insert screenshot** // Docs needed, screen shot (show the button)
- Don't click the "Start WordPress Server" right now, we know it's tempting
    - **info box** 
    - You will see why in a moment

- Click the button to start a new Playground instance
    - **insert screenshot** // Docs needed, screen shot


```bash
mkdir ~/Desktop/working-with-plugins-in-playground && cd $_ && code .
```

- Close the original window, make sure you’re working in the
    - `working-with-plugins-in-playground` directory
    - **insert screenshot**
    
- Clone the repo so you can test out a block
    - `gh repo clone WordPress/block-development-examples`
- Enter the directory and search for a plugin you want to work on
    - `cd block-development-examples/plugins`
- Let’s try out the Interactivity API Countdown block
    - `cd interactivity-api-countdown-3cd73e`
- Start WordPress Server - click me!  // Docs needed, screenshot of button
    - This will launch Playground in **Plugin** mode so you can demo this block
    - **GOTCHA!** Wrong folder // Docs needed, screen flows
        - Stop WordPress Server
- **FIX:** Start completely over 
    - `wp-now stop --reset` // docs needed, do it work work?
    - Deleting the folder and starting over
        - Find the folder in the file system
            - `cd ~/.wp-now`
        - List the contents
            - `ls`
        - Find the folder you just created and delete it
            - `rm -rf ~/.wp-now/{folder-name}`
        - You will notice the folder is named after whatever context you are in 
            - VS Code will open the Playground based on
                - `Playground` mode 
                    - Project you are in has no WordPress context
                    - Creates the default Playground if one doesn't exist in this project context
                - `wp-content` mode
                    - Open the folder and Start WordPress Server
                    - Opens in a Theme and Plugin context
                    - Helpful for including files (`uploads`) 
                    - Good for working on an existing __website__ context
                - `plugin` mode
                    - Project you are in is a plugin
                - `re-open` mode  // AKA "Quirks Mode" - needs docs   
                    - **Note:**  // needs docs, quirky
                    - // loads the same way it did last time
        - `rm -rf ~/.wp-now/*`
    - Open a new VS Code window from this directory
    - `code .`
- Close out the old window for simplicity

## Another way to do it here
- **_Hint:_** Try dragging the folder context into VS Code to open
- You will now have the correct root directory, which you will see in the project URL bar
    - Now click Start WordPress Server
        - You should see a fresh install with the Interactivity API Countdown block available
        - Your block is installed **and activated!**
- Insert the block to test it on a post
    - **Show how to do this programmatically**

## An easier way…

Find the block files, get into that folder as your root project folder, **Launch WordPress Server**

---

## Takeaways…
You have to build and run the block...

Even through the Playground
Everything above won't work until you build the block
- Block doesn’t work without a build step - how to build?
    - Where are the files to build?
    - `wp-scripts` not found…
        - `npm i @wordpress/scripts`
- Block still doesn’t work..
    - Must install interactivity api dependency
- Improvements are coming to this flow

## Testing and Workflows 
- Good for testing      // Docs audit & improve
- Git workflows?        // Docs needed, examples
- Does data persist?    // Docs needed, screen flows

### `wp-now` operations
- How to destroy? `--reset` in `wp-now`
    - (Start from scratch) `wp-now stop --reset`
- How to stop from running? `wp-now stop`
- How to start again? `wp-now start`
- Check to make sure WP Now is stopped
    - `ps aux | grep wp-now` - should return nothing
- Is it building? How to build…
    - Accessing the local filesystem…
    - // docs needed, screenshots

## Next Steps
- Build the block, test in Playground
- //docs needed, screenshots, blueprint.
- Build a blueprint to test a plugin
- Roadmap: VS Code UX improvements