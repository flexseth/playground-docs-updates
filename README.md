## Docs via the Gutenberg Block Editor
Pages here were created in Markdown. The rationale is that Markdown can be pasted into the Block Editor and converted to HTML. 

Markdown is a great syntax for creating
- headings
- intro content (excerpts)
- links - to other documentation, to external resources
- source code

... which allows it to be a great source to enter into the block editor. 

### About pages in this directory
- Each page is a Markdown file
- Pages can be pasted into the Block Editor to create a docs page
- Contributors can then edit the page in the block editor
- PRs can then be used to update the docs (see workflow below)

### How to contribute
A best practice is to create an individual branch for the set of pages or features you want to work on. Use descriptive names like `{feature-name}` 
- [ ] TODO: Add steps to contribute...


### 

## Discussion around meta (Taxonomy)
Finally, add taxonomy to your post so it can be properly categorized and tagged.
- [ ] TODO: Add snippets for the following
- include the `post-tags` block  
- include the `post-categories` block

- TODO: Plugin that Auto Cats and Tags 
    - auto adds the categories and tags to block markup
    Use a block hook to add categories before the post title
    - and block categories appended after the post content. 
    - Add this to the end of your post so the information can be processed correctly (when installed, the categories and tags will be also added in WordPress) when imported via the blueprint.



### Props
- TODO: Add steps for giving [props](https://github.com/adamziel/blueprints/issues/21) to docs contributors
