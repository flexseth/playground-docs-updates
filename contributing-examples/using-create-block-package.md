## Creating a custom block in Playground

Let's say you want to create a new page for a `Blueprint Builder block` feature. 
The feature will be created via a block plugin.

Clone the repo
- [ ] TODO: Add step for cloning the repo

Checkout a new branch to work on locally
IE: `git checkout -b new/playground-bbb`
> `bbb` is the abbreviation for `Blueprint Builder block`
- [ ] TODO: Make the previous line an "info" box in WP

Create the block. 
- TODO: [ ] Add step for navigating to the filesystem
- TODO: [ ] Add step for running `npx @wordpress/create-block playground-bbb`
##### Possible roadblock
- TODO: [ ] Discussion: Is executing via the shell possible in this way right now? [`wp-now` limitation..](./wp-now.md)

Create the functionality for the block. 

Now you want to contribute to documentation, so you need to create a new page in the docs.

This new feature can fall under the `Playground Tools` section. 
- Create your documentation page in the Block Editor
 - title the page `Creating a custom block in Playground`
    - add a heading `Creating a custom block in Playground`
    - add an excerpt `Learn how to create a custom block in Playground`
    - add steps for how to use the feature
    - add example code
    - go to the `Code Editor` and copy the `HTML` code
- Create a new file in the `playground-tools` directory
 - `using-create-block-package.html`
- Paste the HTML code from the Block Editor
- Save the file
- Push your changes to the repo
- Create a PR
- Review the new docs page and feature with the team
- Merge the PR
- [ ] TODO: Props workflow: Receive props for contributing to Playground!
- [ ] TODO: More verbose explanation of the steps above??