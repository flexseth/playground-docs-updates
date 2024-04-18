## Accessibility Testing
https://github.com/adamziel/blueprints/tree/trunk/blueprints/theme-a11y-test

- uses [`a11y-theme-unit-test`](https://github.com/wpaccessibility/a11y-theme-unit-test)
- uses [`theme-test-data`](https://github.com/WordPress/theme-test-data)
- uses [`create-block-theme`](https://wordpress.org/plugins/create-block-theme/)
- uses [`twenty-twenty-four`](https://wordpress.org/themes/twentytwentyfour)

```JSON
{
	"$schema": "https://playground.wordpress.net/blueprint-schema.json",
	"meta": {
		"title": "Theme Tester",
		"description": "Blueprint example to add content and plugins to explore a theme",
		"author": "bph",
		"categories": ["themes", "content"]
	},
	"preferredVersions": {
		"php": "8.0",
		"wp": "beta"
	},
	"features": {
		"networking": true
	},
	"steps": [
		{
			"step": "login"
		},
		{
			"step": "importWxr",
			"file": {
				"resource": "url",
				"url": "https://raw.githubusercontent.com/wpaccessibility/a11y-theme-unit-test/trunk/a11y-theme-unit-test-data.xml"
			}
		},
		{
			"step": "importWxr",
			"file": {
				"resource": "url",
				"url": "https://raw.githubusercontent.com/WordPress/theme-test-data/trunk/themeunittestdata.wordpress.xml"
			}
		},
		{
			"step": "installPlugin",
			"pluginZipFile": {
				"resource": "wordpress.org/plugins",
				"slug": "create-block-theme"
			},
			"progress": {
				"weight": 2
			}
		},
		{
			"step": "installTheme",
			"themeZipFile": {
				"resource": "wordpress.org/themes",
				"slug": "twentytwentyfour"
			},
			"options": {
				"activate": true
			}
		}
	]
}
```