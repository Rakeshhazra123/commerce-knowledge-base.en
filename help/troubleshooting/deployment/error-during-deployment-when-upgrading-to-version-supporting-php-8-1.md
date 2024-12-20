---
title: Error during deployment when upgrading to version supporting PHP 8.1
description: This article provides a solution for the error that occurs during deployment when upgrading to a version that supports PHP 8.1.
exl-id: bdc4a355-4f2b-49a7-9c5d-63c950f7ca30
feature: Deploy, Observability
role: Developer
---
# Error during deployment when upgrading to version supporting PHP 8.1

This article provides a solution for the error that occurs during deployment when upgrading to a version that supports PHP 8.1.

## Affected products and versions

* Adobe Commerce on cloud infrastructure 2.4.4. and later

* Extension or technology (Fastly, New Relic, etc.) version PHP 8.1

## Issue

The following error occurs during deployment when upgrading to a version that supports PHP 8.1.

```PHP
{{E: Error parsing configuration files:

applications: Uncaught exception: The "json" extension is not supported for php:8.1
at <script>:109:12
throw("The \"" + unsupported_extensions[0] + "\" extension is not supported for " + service.type);
^
E: Error: Invalid configuration files, aborting build}}
```

## Cause

PHP 8.1 already includes JSON support and doesn't require the extension to be installed separately.

## Solution

Remove JSON from the **Runtime** > **Extensions** section in `.magento.app.yaml` and redeploy.

## Related reading

[PHP application](https://experienceleague.adobe.com/en/docs/commerce-cloud-service/user-guide/configure/app/php-settings) in our developer documentation.
