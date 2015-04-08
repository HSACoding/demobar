## What?
Demonstration bar to ( themes , websites, plugins ) Beautiful . Original https://github.com/OriginalEXE/Switcheroo

## Demo?
Projeto Testado neste site: [http://hsainformatica.com.br/hsacoding/](http://hsainformatica.com.br/hsacoding/)

## Browsers supported?
It officially supports modern browsers

## Working on mobile/tablets?
iDevices have some serious issues with using iframe this way, that's why bar is automatically closed on tablets/mobile.

## Is it responsive?
Yes, it is.

## Can I use it in commercial purposes?
Not, only apprenticeship.

## How do I add products?
Products are to be added inside products.js file, and assigned to $products global variable. Sample markup:

    $products = {
        visia : {
            name     : 'Visia',
            tag      : 'WP',
            img      : 'http://i.imgur.com/hgp2v0H.jpg',
            url      : 'http://visia.themes.pixelentity.com/',
            purchase : 'http://themeforest.net/item/visia-responsive-one-page-retina-wordpress-theme/5602067?ref=OriginalEXE',
            tooltip  : 'Optional Tooltip'
        },

        bigwig_wp : {
            name     : 'BigWig',
            tag      : 'WP',
            img      : 'http://i.imgur.com/uoreaON.jpg',
            url      : 'http://bigwig.themes.pixelentity.com/',
            purchase : 'http://themeforest.net/item/bigwig-modern-corporate-retina-wordpress-theme/5217458?ref=OriginalEXE'
        }

    };

Note that tooltip is optional, everything else is mandatory.

NOTE: You can now specify if you product should not display viewport buttons, simply add responsive: 0 parameter to the product object in the list above. If not present or value is different, buttons will be showby default for each product.

## How do I specify default product?
Default product will be used if no hash is present. Check products.js for `$current_product = 'visia';`, just replace the visia with the id of your product.

## How do I link to certain product?
You can link to certain product using hashtag + id of the product you want to link to. For example, `http://demourl.com/#bigwig_wp`.
If no product is linked, default product you specified will be displayed.

Note: If you are using this on Envato marketplace, you have to use query string parameter "product" instead because marketplace encodes hash and that causes problem. So on Evato, specify product you are linking to like this: `http://demourl.com/?product=bigwig_wp`


## I would like to customize stuff, how do I get uncompressed source
Uncompressed scripts and styles are included in the package, only they are commented. Simply comment compressed scripts/styled and uncomment uncompressed ones.

## I would like to use image instead of text for the logo, is that supported?
Sure it is. Simply remove 'textual' class from .logo and replace words with your image (optimal height is 60px).

## I hate white color, can I be cool and use black instead?
Of course you can, simply add dark class to the body element and voila.

## How can I contribute?
Find bugs, report bugs, fix bugs.

HSACoding
