Options allow you to pass opinionated data to a blueprint. The data can be used to customize the blueprint's behavior. Options are defined in the blueprint schema and can be accessed in the blueprint steps.

## Hello World
Output Hello World to the console.

```json
{
  "$schema": "https://raw.githubusercontent.com/WordPress/blueprints-library/main/examples/blueprint-schema.json",
  "name": "My Blueprint",
  "description": "This is a blueprint for setting up a WordPress environment.",
  "version": "1.0.0",
  "options": {
    "my_option": {
      "type": "string",
      "title": "My Option",
      "description": "This is an example option.",
      "default": "Hello, World!"
    }
  },
  "steps": [
    {
      "name": "My Step",
      "description": "This is an example step.",
      "type": "shell",
      "command": "echo $MY_OPTION"
    }
  ]
}
``` 