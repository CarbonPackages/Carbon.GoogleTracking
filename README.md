Carbon.GoogleTracking Package for Neos CMS
==========================================

Basically this package gives you some handy prototypes for including Google Tracking and site verification code. The best practice is to include `carbon/googletracking` into your composer.json from your site package. Now you just can edit your Settings.yaml. Take a look at the [Settings.yaml](Configuration/Settings.yaml) to see all the options. If you want to want an automatic integration you have to set  `AddToPagePrototype` in your Settings.yaml to `true`.


Hint
----

If you want to have the tracking only in the Production context, just create a `Production` folder into your  `Configuration` folder. Now create a production only `Settings.yaml` inside that folder. Et voilà! Now you can set your configuration who will only be activated if Neos is in the Production context.


Installation
------------

```
composer require carbon/googletracking
```


License
-------

Licensed under MIT, see [LICENSE](LICENSE)
