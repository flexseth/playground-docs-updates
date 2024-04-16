## Working with `options` in Blueprints
`options` allow you to pass environment data to a blueprint, provided to customize the blueprint's behavior. 

Environment variables are a way to pass dynamic values to a program or script at runtime. They are commonly used to configure and customize the behavior of applications. In the context of the code you provided, options can be passed as environment variables to the blueprint.

To access options as environment variables in the blueprint steps, you can use the syntax `$VARIABLE_NAME`. In the example code, the option `my_option` is accessed using `$MY_OPTION` in the `command` field of the `shell` step.

For more information on environment variables in WordPress, you can refer to the official documentation: [WordPress Environment Variables](https://developer.wordpress.org/cli/commands/config/set/#options-for-environment-variables)

## Definition and scope
Options are defined in the blueprint schema and can be accessed in the blueprint steps.

All options are passed to the environment via a `shell` step in the blueprint.


## Hello World
Output Hello World to the console by passing in a variable

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

## Known Limitations
 `options` are only supported in the online version of the Playground, for now. 
 
 Since `shell` steps cannot be currently utilized by a `WPCLIStep`, because it's currently not supported to run inside the Playground with `options`

 See [WP shell command doesn't work in WP-CLI #1097](https://github.com/WordPress/wordpress-playground/issues/1097)
 