## About the `wpCLI` step
Most any command you can use in the WP-CLI you can use with the Playground.

### Example 1
- [ ] Generate five new posts

## Website migrations with WP-CLI and Playground
- [ ] Performaing a full website migration with WP-CLI
- [ ] Importing a WXR file with WP-CLI
- [ ] Exporting a WXR file with WP-CLI
- [ ] Performing a database search & replace with WP-CLI

## Pass a variable to `wp-cli`
- [ ] Run a `wp-cli` command in a blueprint
```JSON
{
    "name": "Run WP-CLI Command",
    "description": "Run a WP-CLI command in WordPress Playground",
    "inputs": [
        {
            "name": "command",
            "type": "string",
            "description": "The WP-CLI command to run"
        }
    ],
    "runs": {
        "using": "composite",
        "steps": [
            {
                "name": "Set up WordPress Playground",
                "run": "wordpress/playground-setup@v1"
            },
            {
                "name": "Run WP-CLI Command",
                "run": "wordpress/wp-cli@v2",
                "with": {
                    "command": "${{ inputs.command }}"
                }
            }
        ]
    }
}
```
