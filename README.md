# Wordpress plugin for Hostaway
Manage your vacation rental properties like never before with our all-in-one software.

## Pre-production releases:
 * [v1.0-beta-20190903, .zip](https://github.com/Hostaway/wordpress-plugin/releases/download/v1.0-beta-20190903/hostaway-wp-plugin.zip)
 
## Installation

### Installation requirements
 - Required: `php 5.6` and `Wordpress 4.7.0`
 - Recommended: `php 7.2+` and `Wordpress 5.2+`

In case your WordPress is hosted by Wordpress.com, the ability to install plugins requires 
[Business or eCommerce plan](https://en.support.wordpress.com/plan-features/). 

### How to install and configure the plugin
1. Download the latest [hostaway-wp-plugin.zip](https://github.com/Hostaway/wordpress-plugin/releases/download/v1.0-20190827-beta.1/hostaway-wp-plugin.zip)
 and install it: the easiest is to install the plugin through 
[Plugins->Add New->Upload Plugins](https://en.support.wordpress.com/plugins/adding-plugins/#install-plugins-via-a-zip-file), 
or (advanced) upload the plugin files to the `/wp-content/plugins/` directory on the web-server. 
2. On `Plugins` page for `Hostaway` choose `Activate Plugin`. 
3. Use the `Plugins->Hostaway->Settings` page to configure the plugin:
  - Enter your `Account ID` and `Secret code` and press `Get access token` button (it will fetch JWT token used to access Hostaway API).
  - `Google Maps API key` enables using Google Map on the Search and Listing pages.  Get [Google Maps API Key](https://developers.google.com/maps/documentation/javascript/get-api-key).
  - `Google recaptcha public key` and `Google recaptcha private key` are needed to enable recaptcha protection from automated spam. Get [reCAPTCHA API key pair](https://developers.google.com/recaptcha/intro).
  - `Debug mode` helps debug by disabling internal page caching. To turn debugging set to `1`. Once you are happy with results, please remember to set it to `0` for snappier page loads.
  - `Clear cache` momentarily clears internal page and Hostaway API response caches. Currently any Hostaway API response is being cached for 5 mins.
  - If you want to adjust CSS for your theme please go to `Settings->Hostaway->Custom CSS` and paste your styles there.

Now after plugin activation and configuration is done, following new pages in `Pages -> All pages` should be operational:
 - `Hostaway Search Page` - the page with list of all connected listings
 - `Hostaway Listing Details Page` - the listing details page
 - `Hostaway Booking Page` - the booking page
 
 ### How to uninstall the plugin
  - `Settings->Plugins->Hostaway` press `Deactivate` and `Delete`. 
  - Remember, we will be very sorry not to see you using Hostaway wordpress plugin. Please let us know how to improve: 
  [support@hostaway.com](mailto:product@hostaway.com?subject=wordpress%20feedback)
 