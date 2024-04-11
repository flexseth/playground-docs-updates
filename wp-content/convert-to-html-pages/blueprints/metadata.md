## Blueprint Metadata
Each Blueprint should include some basic metadata within the top-level "meta" key in the blueprint.json file. 

Here's what's required:

**Title:** A clear and concise name for your Blueprint.
**Author** (GitHub Username): Let others know who created the Blueprint.
Optionally, you can also include:

**Description**: Provide a brief explanation of what your Blueprint offers.
**Categories**: Specify relevant categories to help users find your Blueprint in the future Blueprints section on WordPress.org.

## Sample metadata
Build a WooCommerce environment that can integrate with WooCommerce CLI (WC-CLI).
```JSON
{
    "meta": {
        "title": "WooCommerce Developer Environment",
        "description": "A local development environment for WooCommerce that includes WC-CLI.",
        "author": "zieladam",
        "categories": ["woocommerce", "developer environment"]
    }
}
```