## Customizing progress bars
When a blueprint is being imported, a standard progress bar will be created. Here's how to customize the look or behavior of the progress of a blueprint.


## TODO: 
- [ ] Add a screenshot of the default progress bar
- [ ] Add examples of how to customize progress bars (look)
- [ ] Add examples of how to customize progress bars (behavior)

## Example: Make progress bar bigger and have a custom caption
```JSON
...
"progress": 
    {
        "weight": 20,
        "caption": "Installing WordPress site"
    }
...
```
via [Playground Plugin PR](https://github.com/WordPress/playground-tools/pull/219#:~:text=%22progress%22%3A%20%7B%0A%20%20%20%20%20%20%20%20%22weight%22%3A%2020%2C%0A%20%20%20%20%20%20%20%20%22caption%22%3A%20%22Installing%20WordPress%20site%22%0A%20%20%20%20%20%20%7D)