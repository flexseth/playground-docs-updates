## How to contribute to Playground docs
1. Fork the repository 
2. Convert Markdown pages to HTML, add content
3. Submit a PR back to the repo with your changes
4. Request review
5. Get props for your work

## Documentation structure
Docs structure is Top Level Page mapped to Top Level Directory, then the single pages are in the directories. The primary "about" pages are in the primary /wp-content/html-pages folder, these pages provide links to longer form docs pages when necessary. Or to other relevant documentation pages in the WordPress ecosystem.

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
- Performaing a full website migration with WP-CLI
- Importing a WXR file with WP-CLI
- Exporting a WXR file with WP-CLI
- Performing a database search & replace with WP-CLI
```
##### Instead, do this
```markdown
## Website migrations with WP-CLI and Playground
- Performaing a full website migration
- Importing a WXR file
- Exporting a WXR file
- Performing a database search & replace
```

In this example doc, it's assumed that the list is using the `WP-CLI` utility