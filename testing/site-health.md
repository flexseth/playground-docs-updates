## Site Health reports
The site health feature is now enabled in Playground 🎉 You can try it out here:

https://playground.wordpress.net/?networking=yes&url=/wp-admin/site-health.php?tab=debug


## Known Limitations
The support is not full yet as Playground does not support PHP making HTTP requests to itself (e.g. wp_safe_remote_get("https://playground.wordpress.net/scope:0.0875753914918784/index.php?rest_route=%2Fwp%2Fv2%2Ftypes%2Fpost&context=edit"), which is something the Site Health report does. Once that feature is supported, the site health report should be fully functional.

This isn't directly related to the core of this issue which is to start Playground based on an existing site health report, but I felt it was relevant to share here anyway.

## Request for feedback
How to send an automatic site health report with all relevant site data, securely, to a support team. Related to 

## Feature ideas
Blueprint for Deep Linking to Site Health page and sending reports
Blueprint to Site Health page with a built-in report 