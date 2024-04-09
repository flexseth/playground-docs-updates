## Requirements
`wp-now` includes an entire WordPress environment, so you don't need to install WordPress separately. It runs on PHP WASM...

## Limitations
The `shell` step currently won't work in `wp-now` because it doesn't support the `shell` command.
This is a known limitation that we are working towards making work! 
- [ ] TODO: Clarify what common "shell" type things you can do another way in `wp-now`

## Security warnings
Sometimes when you use packages from an external source, the project you are using needs to update them. 

See the [Security Warnings](./playground-tools/wp-now/fixing-security-warnings.md) page for more information on how to audit and fix security issues in `wp-now`.
- [ ] TODO: Update docs with how to audit and fix security issues in `wp-now`