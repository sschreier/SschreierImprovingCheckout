# An extension to improve the checkout for Shopware 6

An extension to _improve the checkout_.

For example, the _visitor can be shown a progress bar_ (based on the **Bootstrap Progress** component) _in off canvas shopping cart and the normal shopping cart_, which _shows in real time the remaining amount until free shipping_. If necessary, you can _change the background color of the progress bar_ and the _progress_. In addition, an _animation can be displayed in the progress bar_ and a _truck icon can be displayed before the text_. 

It is also possible to _hide the input field for a voucher code in off canvas shopping cart and the normal shopping cart_. 

The _display of_ the _input field for a product number can_ also _be prevented in the normal shopping cart_.

## how to use it

### shipping method settings

1. go to "**Settings**", "**Shop**" and "**Shipping**" and open a shipping method, for example  "**Standard**"
2. switch to the area "**Unrestricted**"
3. select the property "**Cart price**" for the price matrix
4. add a pricing level via the button "**Add pricing level**" for a cart price for example from "**0**" to "**38.99**" euro with "**3.99**" euro shipping costs
5. add a second pricing level for a cart price from "**39**" euro to "**infinite**" with "**0**" euro shipping costs
6. click on the button "**Save**"

## Possible configurations for the free shipping progress bar
- select if the free shipping progress bar should be shown in the off canvas shopping cart
- select if the free shipping progress bar should be shown in the shopping cart
- select the background color of the progress bar (*1)
- select the background color of the progress (*1) 
- select if an animation should be shown
- set the text of the hidden headline via snippet
- select if a truck icon should be shown before the text
- set the text until free shipping is reached via snippet
- select if the success message should be shown
- set the text when reaching free shipping via snippet

## Possible configurations for the input field for a voucher code
- select if the input field should be shown in the off canvas shopping cart
- select if the input field should be shown in the shopping cart

## Possible configurations for the input field for a product number
- select if the input field should be shown in the shopping cart

## Available snippets
- sschreier.improvingcheckout.freeShippingProgressBar.headline
- sschreier.improvingcheckout.freeShippingProgressBar.textUntilIsReached
- sschreier.improvingcheckout.freeShippingProgressBar.isReached

## Some changes in the settings within the configuration are not immediately visible in the frontend of the shop
After changing settings specifically for the appearance of the free shipping progress bar (*1), the theme must be recompiled, for example by saving the theme in the administration:
1. Switch to "Content" and "Themes"
2. Select the active theme
3. Click on the button "Save"

## How to install the extension
### via zip and console (recommended)
1. Download the latest _SschreierImprovingCheckout-master.zip_.
2. Unzip the zip file and rename the folder to _SschreierImprovingCheckout_.
3. Move the folder to the project folder _custom/plugins/_ .
4. Connect to the console via ssh:

```
bin/console plugin:refresh
bin/console plugin:install --activate SschreierImprovingCheckout
```

### via composer
1. Add the repository URL to the composer.json of the project
```
"repositories": [
    ...,
    {
        "type": "vcs",
        "url": "https://github.com/sschreier/SschreierImprovingCheckout"
    }
],
```

2. Connect to the console via ssh and install the plugin via the command
```
composer require sschreier/sschreierimprovingcheckout
bin/console plugin:refresh
bin/console plugin:install --activate SschreierImprovingCheckout
```

### via https://packagist.org
- Connect to the console via ssh and install the plugin via the command
```
composer require sschreier/sschreierimprovingcheckout
bin/console plugin:refresh
bin/console plugin:install --activate SschreierImprovingCheckout
```

### via zip upload
1. Download the latest _SschreierImprovingCheckout-master.zip_.
2. Unzip the zip file and rename the folder to _SschreierImprovingCheckout_.
3. Zip the folder to _SschreierImprovingCheckout.zip_.
4. Upload the zip in the Shopware Administration.
5. Install & Activate the extension.

#### extension update (zip)
1. Download the latest _SschreierImprovingCheckout-master.zip_.
2. Unzip the zip file and rename the folder to _SschreierImprovingCheckout_.
3. Zip the folder to _SschreierImprovingCheckout.zip_.
4. Upload the zip in the Shopware Administration.
5. Update the extension.

## Images

### free shipping progress bar in the off canvas shopping cart

![free shipping progress bar in the off canvas shopping cart](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image1.jpg)

### free shipping progress bar in the normal shopping cart

![free shipping progress bar in the normal shopping cart](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image2.jpg)

### success message in the normal shopping cart

![success message in the normal shopping cart](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image3.jpg)

### free shipping progress bar in the normal shopping cart with discount

![free shipping progress bar in the normal shopping cart with discount](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image4.jpg)

### free shipping progress bar in the normal shopping cart with input field for a voucher code

![free shipping progress bar in the normal shopping cart with input field for a voucher code](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image5.jpg)

### free shipping progress bar in the normal shopping cart with input field for a product number

![free shipping progress bar in the normal shopping cart with input field for a product number](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image6.jpg)

### free shipping progress bar in the normal shopping cart with a free shipping product

![free shipping progress bar in the normal shopping cart with a free shipping product](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image7.jpg)

### extension configuration part 1

![extension configuration part 1](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image8.jpg)

### extension configuration part 2

![extension configuration part 2](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image9.jpg)

### extension configuration part 3

![extension configuration part 3](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image10.jpg)

### extension configuration part 4

![extension configuration part 4](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image11.jpg)

### shipping method settings

![shipping method settings](https://www.sebastianschreier.de/plugins/SschreierImprovingCheckout/SschreierImprovingCheckout-Image12.jpg)
