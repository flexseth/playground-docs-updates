## How to contribute to Playground docs
How to help update the Playground documentation

1. Fork the repository 
2. Checkout a branch you want to work on or make commits
3. Make changes using feature or update branches
    - IE: `feature/{feature-name}` or `update/{update-name}`
4. Submit a pull request
    - PRs should be descriptive and include the issue number
    - PRs should include a description of the changes
5. Review the PR
    - PRs will be reviewed by the Playground team
    - PRs will be merged by the Playground team

## Documentation structure
The folder structure is top level "index" style page in the root directory, and then sub-directories represent features.

The directory structure is `/feature/README.md` or some other index files for the feature.

If a file is in the root level of the directory, it's assumed to be a top-level page. 

These will be overview pages that link to other pages in the directory. Or to other relevant documentation.

## Documentation standards
- Index pages
- - directory (folder)
- - - sub-page

---

## Formatting best practices
Readability - try to not overuse words in Markdown
##### Don't do this
```markdown
## Website migrations with WP-CLI and Playground
Notice the redundancy in the list items below
- Performaing a full website migration with WP-CLI
- Importing a WXR file with WP-CLI
- Exporting a WXR file with WP-CLI
- Performing a database search & replace with WP-CLI
```
##### Instead, write the doc more concisely
```markdown
## Website migrations with WP-CLI and Playground
- Performaing a full website migration
- Importing a WXR file
- Exporting a WXR file
- Performing a database search & replace
```

In this example doc, it's assumed that the list is using the `WP-CLI` utility, make sure to note any limitations issues.

## Work in Progress
This file is a work in progress

## Roadmap
Error and Issue templates