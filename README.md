Carbon.GoogleTracking Package for Neos CMS
==========================================
[![Latest Stable Version](https://poser.pugx.org/carbon/googletracking/v/stable)](https://packagist.org/packages/carbon/googletracking)
[![Total Downloads](https://poser.pugx.org/carbon/googletracking/downloads)](https://packagist.org/packages/carbon/googletracking)
[![License](https://poser.pugx.org/carbon/googletracking/license)](LICENSE)

This package gives you some handy prototypes for including Google Tracking and site verification code. The best practice is to include `carbon/googletracking` into your composer.json from your site package. Now you just can edit your Settings.yaml. Take a look at the [Settings.yaml](Configuration/Settings.yaml) to see all the options. If you want to want an automatic integration, you have to set  `AddToPagePrototype` in your Settings.yaml to `true`.


Hint
----

If you want to have the tracking only in the Production context, just create a `Production` folder into your  `Configuration` folder. Now create a production only `Settings.yaml` inside that folder. Et voilà! Now you can set your configuration which will only be activated if Neos is in the Production context.


Installation
------------

Most of the time you have to make small adjustments to a package (e.g. configuration in `Settings.yaml`). Because of that, it is important to add the corresponding package to the composer from your theme package. Mostly this is the site packages located under `Packages/Sites/`. To install it correctly go to your theme package (e.g.`Packages/Sites/Foo.Bar`) and run following command:
```
composer require carbon/googletracking --no-update
```

The `--no-update` command prevent the automatic update of the dependencies. After the package was added to your theme `composer.json`, go back to the root of the Neos installation and run `composer update`. Et voilà! Your desired package is now installed correctly.


License
-------

Licensed under MIT, see [LICENSE](LICENSE)
