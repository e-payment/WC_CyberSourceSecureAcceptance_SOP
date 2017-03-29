## Installation

 * Upload the plugin files to the '/wp-content/plugins/' directory
 * Activate the plugin through the 'Plugins' menu in WordPress
 * Go to your WooCommerce payment Gateway settings page and enable/configure the gateway

## Configuration

### To configure the plugin

 * First, ensure that Secure Acceptance Silent Order Post is enabled for your cybersource account
 * Create a Profile Id: log into the CyberSource Business Center and go to Tools & Settings > Profiles > Create New Profile
 * Generate an Access Key : log into the CyberSource Business Center and go to Tools & Settings > Profiles > Profile Name > Security > Create New Key > Give it a Name > Generate Key
 * Generate a Secret Key: log into the CyberSource Business Center and go to Tools & Settings > Profiles > Profile Name > Security. The Secret Key is automatically generated from the previous step.
 * Make sure to disable test/debug modes in the WooCommerce Settings page prior to accepting live transactions!

### To configure CyberSource

 * Log into the CyberSource Business Center
 * Go to Tools & Settings > Profiles > Profile Name > Payment Settings.
 * Click 'Save' at the top\bottom of the page.
 * Ensure that the supported Credit\Debit Cards are added to the Payment Method list that you selected in the WooCommerce plugin settings are also listed.
 * Under 'Customer Response Pages' set the 'Hosted by you URL' to https://www.example.com/?wc-api=wc_gateway_cybersource_secure_acceptance_sop_response where www.example.com is the host name of your server
 * Click 'Save' at the top\bottom of the page.

## Testing
 
### For test transactions

```
* Card Type/Number:
  Visa                4000 0000 0000 0002
  MasterCard          5555 5555 5555 4444
  Maestro Int'l       6000 3400 0000 9859
  American Express    378  2822 4631 0005
 
* Expiration Date: any date in the future
* Card Security Code: any 3 digits
```