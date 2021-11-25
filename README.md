
# Facebook Business Extension For Magento2

## Facebook Connects Businesses with People

Marketing on Facebook helps your business build lasting relationships with people, find new customers and increase sales for your online store. With this Facebook ad extension, we make it easy to reach the people who matter to your business and track the results of your advertising across devices. This extension will help you:

### Reach the right people
Set up the Facebook pixel to find new customers, optimize your ads for people likely to buy and reach people with relevant ads on Facebook after they've visited your website.

### Show them the right products
Connect your product catalog to Facebook to use dynamic ads. Reach shoppers when they're on Facebook with ads for the products they viewed on your website.

### Measure the results of your ads
When you have the Facebook pixel set up, you can use Facebook ads reporting to understand the sales and revenue that resulted from your ads.
Many online retailers have found success using the Facebook pixel to track the performance of their ads and run dynamic ads:

“The ability to measure sales was the first sign that our business would be a success. Our first day of breaking 100-plus sales always sticks out. Point blank, our marketing plan is Facebook, Facebook, and more Facebook... Facebook is 100% the backbone of our customer acquisition efforts and it's been made even better with the improved Facebook pixel” — Ali Najafian, co-founder, Trendy Butler

“I'm thrilled with the results we've seen since launching dynamic ads. We saw a rise in conversions almost immediately after launch and have been able to scale the program at an impressive pace over the past 6 months. These ads have proven to be a key component of our marketing efforts” — Megan Lang, Digital Marketing Manager, Food52

“With dynamic ads, Target has been able to easily engage consumers with highly relevant creative. The early results have exceeded expectations. Performance has been especially strong on mobile devices — an important and fast-growing area for Target — where we're seeing two times the conversion rate” — Kristi Argyilan, Senior Vice President, Media and Guest Engagement at Target

## What's included?

### (a) Pixel installer
Installing the Facebook pixel allows you to access the features below:

Conversion tracking: See how successful your ad is by seeing what happened as a direct result of your ad (including conversions and sales)

Optimization: Show your ads to people most likely to take a specific action after clicking on them, like adding an item to their cart or making a purchase

Remarketing: When people visit your website, reach them again and remind them of your business with a Facebook ad

### (b) Product catalog integration
Importing your product catalog to Facebook allows you to use dynamic ads. Dynamic ads look identical to other link ads or carousel-format ads that are available on Facebook. However, instead of individually creating an ad for each of your products, Facebook creates the ads for you and personalizes them for each of your customers.

Scale: Use dynamic ads to promote all your products without needing to create individual ads for each item

Highly relevant: Show people ads for products they're interested in to increase the likelihood of a purchase

Always-on: Set up your campaigns once and continually reach people with the right product at the right time

Cross-device: Reach people with ads on any device they use, regardless of where they first see your products


## Usage Instructions

Facebook Business Extension - Installation steps

INSTALL FACEBOOK BUSINESS EXTENSION FROM ZIP FILE ON YOUR DEV INSTANCE. TEST THAT THE EXTENSION
WAS INSTALLED CORRECTLY BEFORE SHIPPING THE CODE TO PRODUCTION

Before installing, verify your Magento cron job is up and running, read more about it on [this](https://devdocs.magento.com/guides/v2.3/config-guide/cli/config-cli-subcommands-cron.html) page.

Login to your server instance.

### INSTALLATION

#### Composer Installation
We recommend installing the extension using Composer since it makes it easy to update, or uninstall the extension.

* Go to your magento root path
* Execute command `cd /var/www/Magento` or
 `cd /var/www/html/Magento` based on your server Centos or Ubuntu.
* run composer command: `composer require facebook/facebook-for-magento2`
- To enable module execute `php bin/magento module:enable Facebook_BusinessExtension`
- Execute `php bin/magento setup:upgrade`
- Optional `php bin/magento setup:static-content:deploy`
- Execute `php bin/magento setup:di:compile`
- Execute `php bin/magento cache:clean`
- Execute `php bin/magento cron:run` three times

### Verify Installation
- Upon successful installation, login to your Magento Admin panel.
- Click the Stores icon in the main menu.
- There should be a section named Facebook -> Setup
- Click on 'Setup' to go to the Extension Installation Page.

### Unistall 
Move to the Magento root directori and execute:
`php bin/magento module:uninstall -r Facebook_BusinessExtension`

### Catalog sync
By default the catalog sync is enabled, you can push products, or product categories to Facebook, or turn off the catalog sync.
To set up the catalog, log into the admin panel.
Navigate to: Store > Configuration > Facebook > Business Extension 


## Testing before installing

If you want to test this extension in a separate environment, without making changes in your production server, you can use the files provided in tests folder.

Follow `docker-installation-instructions.txt` file to run a Magento 2 store with the extension installed, using Docker, so you can test in your local machine.

## Need help?

Visit Facebook's [Advertiser Help Center](https://www.facebook.com/business/help/532749253576163).

## Requirements

Facebook Business Extension For Magento2 requires
* Magento version 2.0 and above
* PHP 7.0 or greater
* Memory limit of 1 GB or greater (2 GB or higher is preferred)

## Contributing

See the CONTRIBUTING file for how to help out.

## License

Facebook Business Extension For Magento2 is Platform-licensed.
