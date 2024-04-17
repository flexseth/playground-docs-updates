## Using comments in Blueprints
Written in `JSON` format, Blueprints do not support comments. However, there are a few ways you can add comments to your Blueprints:

### If the Blueprint is listed on the Community Gallery
- You can use a `runPHP` step with `/* */` comments to add comments to your Blueprint.
- You can link the Blueprint `meta data` to a GitHub repository and use GitHub comments.

### If you have the blueprint in your repository
If you would like to use comments to fully explain how your blueprint works, a good way to do this is via a `README.md` file to explain step-by-step.

### Using the `blueprint.md` file to to add comments
If you have a `blueprint.md` file in your blueprint directory, you can use this file to add comments to your Blueprint. This file is not used by the Blueprint itself, but it can be used to add comments to the Blueprint. 

It will be displayed in the Blueprint editor and can be used to explain the Blueprint to other users.
- TODO: Discuss the following file structure
 - `blueprint-directory-name`
 - `blueprint-directory-name/blueprint.json`
 - `blueprint-directory-name/blueprint.md`
- TODO: Plugin previews with comments
 - see the [following file structure](https://github.com/ockham/like-button/tree/trunk/_playground)
