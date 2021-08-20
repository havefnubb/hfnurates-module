Hfnurates module
==================

This is a module for Jelix, to rate some data like news or products.

This module is for Jelix 1.7.2 and higher.

It was originally developped into the [Havefnubb project](https://github.com/havefnubb/havefnubb/).

Setting up the module
=====================

The best method is to use Composer.

In a commande line inside your project, execute:

```
composer require "havefnubb/hfnurates-module"
```

Launch the configurator for your application to enable the module

```bash
php dev.php module:configure hfnurates
```

After configuring the module, you should launch the installer of your application
to activate the module:

```bash
php install/installer.php
```

You should attach url of hfnurates to the main entrypoint of your
application. Exemple, in your `app/system/urls.xml`:

```xml
<classicentrypoint name="index" default="false" noentrypoint="false">
    ...
    <url pathinfo="/rates" module="hfnurates" include="urls.xml"/>
    ...
</classicentrypoint>

```
