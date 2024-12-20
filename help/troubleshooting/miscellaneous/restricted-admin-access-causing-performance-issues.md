---
title: Restricted admin access causing performance issues
description: This article provides solutions for when performance is negatively impacted by using [Admin roles with role scope restricted by website](https://experienceleague.adobe.com/en/docs/commerce-admin/systems/user-accounts/permissions-user-roles#step-2assign-resources) in our user guide.
exl-id: da168d6b-9cda-41e2-aa3c-f3f0dccc803d
feature: Admin Workspace, Cache
role: Developer
---
# Restricted admin access causing performance issues

This article provides solutions for when performance is negatively impacted by using [Admin roles with role scope restricted by website](https://experienceleague.adobe.com/en/docs/commerce-admin/systems/user-accounts/permissions-user-roles#step-2assign-resources) in our user guide.

## Affected products and versions

* Adobe Commerce on-premises 2.2.x, 2.3.x
* Adobe Commerce on cloud infrastructure 2.2.x, 2.3.x

## Issue

When an Admin user, with the role scope restricted by website, performs operations in the Admin panel (including logging in, saving products and so on), Adobe Commerce rebuilds the stored cache. Rebuilding the cache negatively impacts performance and can lead to a site outage, especially during business and/or high-traffic hours.

The issue is fixed in Adobe Commerce 2.2.10 and 2.3.3.

## Solution

Following are the options to avoid the issue:

* Upgrade the Adobe Commerce application version to 2.2.10 or 2.3.3. (for instructions, see the [Upgrade Adobe Commerce on cloud infrastructure version](https://experienceleague.adobe.com/en/docs/commerce-cloud-service/user-guide/develop/upgrade/commerce-version) in our developer documentation).
* Avoid restricting Admin user role scope by website, if possible.
* [Submit a Magento Support ticket](/help/help-center-guide/help-center/magento-help-center-user-guide.md#submit-ticket), to request a patch, if it is available.

## Related reading

* [User roles](https://experienceleague.adobe.com/en/docs/commerce-admin/systems/user-accounts/permissions-user-roles) in our user guide.
