# Mapp Connect APIs Client Library for PHP #

## Overall information ##

*PHP-Client* project is a middleware between *MappConnect* and *Shopware plugin*
to execute basic events:

* connection status
* get messages
* get groups
* execute specified events for given *integrationId*

## Installation ##

1. If upgrading from previous version please remember to update database
`bin/console database:migrate MappConnect --all`

Clear shopware cache
`bin/console cache:clear`

And deploy new UI assets
`bin/console asset:install`

2. *php-client* needs to be installed within *Shopware plugin*
* The project needs at least of php version 7.0 * 

3. In the *Shopware plugin* you should first get *php-client* which you can install within *plugin* folder (in Shopware 6 you should go to path `/src/custom/plugins/[shopware_plugin_name]`), and then run `composer install`,

4. *Shopware plugin* you can activate by 

4a. Going to *Administration* section in Shopware, and next go to *Settings->System->Plugins* and from the list **Install** ( you can also **Configure** it from context menu), and next **Activate** this within toggle button,

4b. You can also activate this from the Shopware console by:

* `php bin/console plugin:refresh`
* `php bin/console plugin:install --activate MappConnect`

And you can now use Plugin along with all events support in relation to Mapp Connect.