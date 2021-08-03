# Mapp Connect APIs Client Library for PHP #

## Overall information ##

*PHP-Client* project is a middleware between *MappConnect* and *Shopware & Magetno plugin*
to execute basic events:

* connection status
* get messages
* get groups
* execute specified events for given *integrationId*

## Installation ##

1. *php-client* needs to be installed within *Shopware & Magento plugin*
* The project needs at least of php version 7.0 * 

2. In the *Shopware plugin* you should first get *php-client* which you can install within *plugin* folder (in Shopware 6 you should go to path `/src/custom/plugins/[shopware_plugin_name]`), and then run `composer install`,

3. *Shopware plugin* you can activate by 

3a. Going to *Administration* section in Shopware, and next go to *Settings->System->Plugins* and from the list **Install** ( you can also **Configure** it from context menu), and next **Activate** this within toggle button,

3b. You can also activate this from the Shopware console by:

* `php bin/console plugin:refresh`
* `php bin/console plugin:install --activate MappConnect`

And you can now use Plugin along with all events support in relation to Mapp Connect.
