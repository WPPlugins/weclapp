=== weclapp ===
Contributors: Lukas Kröger
Tags: webinar, weclapp, campaign, cloud, ERP, CRM, ticketing, helpdesk
Requires at least: 4.0
Tested up to: 4.7
Stable tag: 1.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This plugin integrates weclapp functionality into wordpress CMS

== Description ==

<h4> Campaign Management </h4>

Adds the possibility to display campaigns and allow automatic webinar registration. It integrates the following two elements into your webpage:

* a list of upcoming campaigns of a chosen type scheduled in your weclapp account under CRM -> campaigns
* a display of a submit form enabling visitors of your website to participate in one or more campaigns with one single registration (this feature can be deactivated using the Shortcode parameter <code>displayformular=0</code>)

If a user is not in your contact, lead, or customer list in weclapp then then the participant will be added to your contacts (contact type can be set in the Plugin Settings under "Create new persons as").

Participants trying to register repeatedly will be informed about their already existing participation. 

Additional features: 

* success messages can be configured under the plugin settings
* multiple formulars or lists on one page 

Here is a sample how the usage of the plugin looks like: https://www.weclapp.com/de/webinare/

<h4> Ticket Management </h4>

Allows the visitors of your webpage to send a support query by means of a submit formular. The request will be automatically included in your ticket list accessible under Helpdesk in your weclapp account.

<h4> More functionality will be added in the future </h4>

<h4> Supported languages: </h4>

* German
* English
* French
* Spanish
* Turkish
* Polish

If you encounter translation mistakes, feel free to inform us at the following email-address: support[@]weclapp.com

== Example Usage ==

<h4> Campaign Management </h4>

To use this feature, just place the Shortcode <code>[weclappCampaings]</code> into a chosen post. 

By default webinar is the campaign type. If you like to use another campaign type, use the Shortcode parameter <code>type</code>. It is also possible to disable the formular using the Shortcode parameter <code>displayformular=0 </code>. 

For instance, if you like to list all upcoming events without a formular:

<code> [weclappCampaigns type="Event" displayformular=0] </code>

Use the following names for the campaign types:

* Event
* Webinar
* Exposition 
* Publicrelation
* Advertisement
* Bulkmail
* Email
* Telemarketing
* Other

Multiple formulars on one page (with different campaign types respectively) can easily be created by placing multiple Shortcodes on it.

<h4> Ticket Management </h4>

The only thing necessary is inserting the shortcode <code>[weclappTicketing]</code> into one of your posts. 
Optionally, you can add the following fields to the formular using the shortcode parameters in brackets:

* phone number (<code>phone_number=1</code>)
* additional recipients (<code>additional_recipients=1</code>)
* category (<code>category=1</code>)

For example, the following shortcode will display the submit formular including a category select box:

<code>[weclappTicketing category=1]</code>  

If you encounter any errors messages, check your plugin settings as shown under "Installation".

== Installation ==

1. Download and install plugin under Plugins -> Add new.
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Setup your plugin (API data in weclapp can be found under the user settings):
  * Enter your API Token
  * Enter your domain name e.g. your_domain_name.weclapp.com (without "https://")


== Screenshots ==

For an impression visit https://www.weclapp.com/de/webinare/

1. Plugin settings

2. List of all campaigns with type webinar with one opened description

3. List of all campaigns with type webinar including a formular

4. Support request formular

== Changelog ==

1.0 Initial version with campaign support only

1.1 Shortcode parameters added and settings modified

1.2 Ticket Management added, shortcode parameters changed 

1.3 Compatibility with wordpress 4.7

== Upgrade Notice ==

1.1 Update to this version to use all kinds of campaigns and more than one weclapp-Shortcodes on one page.

1.2 Update to this version to use Ticket Management 

1.3 Compatibility with wordpress 4.7