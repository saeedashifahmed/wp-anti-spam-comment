=== WP Anti-Spam Comment ===
Contributors: saeedashifahmed
Donate link: https://rabbitbuilds.com/
Tags: anti spam, stop spam, comment spam, security, gdpr
Requires at least: 5.0
Requires PHP: 7.4
Tested up to: 6.7
Stable tag: 2.0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Advanced, lightweight, and GDPR-compliant anti-spam protection for WordPress comments. Zero configuration needed.

== Description ==

The fastest and most comprehensive GDPR-compliant Anti-Spam plugin to prevent bot spam in the **Default Commenting System** of WordPress. Formerly known as "Forget Spam Comment" — now with multi-layer protection and a modern settings dashboard.

== Important ==
* Please clear page cache after plugin activation.
* Only for the default commenting system. Not for AMP.

= Features =
* 🛡️ **Hash-Based Verification** — Blocks bots by hiding the comment form action URL
* 🍯 **Honeypot Trap** — Hidden field that catches bots filling every input
* ⏱️ **Time-Based Check** — Rejects comments submitted too quickly
* 🔒 **REST API Protection** — Blocks unauthenticated REST API comments
* 📊 **Spam Statistics Dashboard** — Real-time total & daily blocked spam counter
* ⚙️ **Modern Settings Page** — Beautiful card-based UI with toggle switches
* 🔔 **Admin Bar Counter** — See blocked spam count in the admin bar
* ✏️ **Custom Block Message** — Personalize the blocked spam response
* 100% GDPR Compliant — No external requests, no cookies, no tracking
* Captcha-Free — Completely invisible to your visitors
* ~200 bytes inline JavaScript — Zero performance impact
* Compatible with all page caching and performance optimization plugins

= How does it work? =
1. The comment form action URL is removed from the HTML
2. Real user interactions (scroll, mouse move, touch, focus) trigger JavaScript to restore the URL with a unique hash token
3. Server validates the hash, checks the honeypot, and verifies timing
4. Failed validations get a 403 response — no spam ever reaches your database

== Installation ==

To install from the WordPress Dashboard:

1. Go to Plugins menu > Add New
1. Search for WP Anti-Spam Comment
1. Activate the plugin
1. If using a page cache, clear/purge the cache

To install manually:

1. Download the WP Anti-Spam Comment plugin
1. Upload to the `/wp-content/plugins/` directory
1. Activate through the 'Plugins' menu
1. If using a page cache, clear/purge the cache

== Frequently Asked Questions ==

= How to configure the plugin? =
Navigate to Settings > WP Anti-Spam to toggle protection modules, set timing thresholds, and view spam statistics.

= How to test whether the plugin is working? =
Go to any post where comments are enabled and try posting a comment. If it goes through successfully, everything is working. If you see error 403, clear your page cache. If comments still fail, your theme may use a non-standard comment form ID — please open a support topic.

= Which commenting system is supported? =
Only the Default Commenting System of WordPress. Disqus, JetPack Comments, wpDiscuz, and AMP comments are not supported.

= How to get technical assistance? =
Please open a support topic. We will reply within 24 hours.

== Changelog ==

= 2.0.1 =
* **Major Rebrand** — Renamed from "Forget Spam Comment" to "WP Anti-Spam Comment"
* **New:** Honeypot trap field for catching bots
* **New:** Time-based submission check (configurable threshold)
* **New:** REST API comment protection
* **New:** Modern settings page with card-based UI and toggle switches
* **New:** Real-time spam statistics (total, today, last blocked)
* **New:** Admin bar spam counter
* **New:** Custom blocked message setting
* **New:** Reset to defaults button
* **New:** Expanded event triggers (scroll + mousemove + touchstart + focus)
* **New:** Expanded comment form ID selector for more theme compatibility
* **Improved:** Block response page with modern, branded design
* **Improved:** Activation notice with modern styling
* **Updated:** Requires WordPress 5.0+ and PHP 7.4+

= 1.1.8 =
* Tested with 6.6.1 Updated on 09-Aug-2024.

= 1.1.7 =
* Tested with 6.5.5 Updated on 09-July-2024.

= 1.1.6 =
* Hotfix for Bedrock Compatibility. Updated on 30-Jan-2024.

= 1.1.5 =
* Enhanced Bedrock Compatibility. Updated on 24-Jan-2024.

= 1.1.4 =
* Added a fallback to cover unexpected cases. Updated on 20-Nov-2023.

= 1.1.3 =
* Enhanced uniqueness in query string parameters. Updated on 19-Nov-2023.
* Kindly clear your page cache after updating to version 1.1.3.

= 1.1.2 =
* Tested with WordPress 6.4.1 and PHP 8.2.12
* Addressed referral handling for increased precision
* Improved code readability and consistency following WordPress coding standards

= 1.1.1 =
* Tested with WordPress 6.2 and PHP 8.2.4

= 1.1.0 =
* Tested with WordPress 6.1.1 and PHP 8.2.3
* Updated links

= 1.0.9 =
* Tested with WordPress 6.0

= 1.0.8 =
* Tested with WordPress 5.9.1 and PHP 8.1.3

= 1.0.7 =
* Tested with WordPress 5.8
* Enhanced compatibility

= 1.0.6 =
* Tested plugin up to 5.7

= 1.0.5 =
* Added hint for purging cache in the generated error page to assist first time plugin user.

= 1.0.4 =
* Minor tweaks

= 1.0.3 =
* Minified inline JS for better performance
* Translation made available for Hindi, Bengali, English (United States), English (UK).
* Minor tweaks

= 1.0.2 =
* Added hint for purging cache upon plugin activation
* Added support links

= 1.0.1 =
* Performance optimization

= 1.0.0 =
* Initial release

== Upgrade Notice ==

= 2.0.1 =
**Major update!** Rebranded as "WP Anti-Spam Comment" with new honeypot, time-check, REST API protection, and modern settings page. Please deactivate and reactivate the plugin, then clear your page cache.