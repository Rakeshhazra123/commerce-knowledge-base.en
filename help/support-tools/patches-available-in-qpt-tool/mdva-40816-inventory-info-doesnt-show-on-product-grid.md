---
title: "MDVA-40816: Inventory data not shown on product grid"
labels: QPT patches,Quality Patches Tool,Support Tools,QPT 1.1.10,Magento,Adobe Commerce,cloud infrastructure,on-premises,inventory,2.3.0,2.3.1,2.3.2,2.3.2-p2,2.3.3,2.3.3-p1,2.3.4,2.3.4-p2,2.3.5,2.3.5-p1,2.3.5-p2,2.3.6,2.3.6-p1,2.3.7,2.3.7-p1,2.3.7-p2,2.4.0,2.4.0-p1,2.4.1,2.4.1-p1,2.4.2,2.4.2-p1,2.4.2-p2,2.4.3,2.4.3-p1
description: "The MDVA-40816 patch solves the issue where inventory information is not displayed on the product grid if a product SKU contains special characters. This patch is available when the [Quality Patches Tool (QPT)](https://support.magento.com/hc/en-us/articles/360047139492) 1.1.10 is installed. The patch ID is MDVA-40816. Please note that the issue is scheduled to be fixed in Adobe Commerce 2.4.5."
---

# MDVA-40816: Inventory data not shown on product grid

The MDVA-40816 patch solves the issue where inventory information is not displayed on the product grid if a product SKU contains special characters. This patch is available when the [Quality Patches Tool (QPT)](https://support.magento.com/hc/en-us/articles/360047139492) 1.1.10 is installed. The patch ID is MDVA-40816. Please note that the issue is scheduled to be fixed in Adobe Commerce 2.4.5.

## Affected products and versions

**The patch is created for Adobe Commerce version:**

* Adobe Commerce (all deployment methods) 2.4.3

**Compatible with Adobe Commerce versions:**

* Adobe Commerce (all deployment methods) 2.3.0 - 2.4.3-p1

>[!NOTE]
>
>The patch might become applicable to other versions with new Quality Patches Tool releases. To check if the patch is compatible with your Adobe Commerce version, update the `magento/quality-patches` package to the latest version and check the compatibility on the [QPT landing page](https://devdocs.magento.com/quality-patches/tool.html#patch-grid). Use the patch ID as a search keyword to locate the patch.

## Issue

Inventory data is not displayed on the product grid if a product SKU contains special symbols.

<u>Prerequisites</u>:

MSI is installed.

<u>Steps to reproduce</u>:

1. Create a simple product.
1. Modify a product's SKU to include special symbols such as & or '.
1. Open the product grid.

<u>Expected results</u>:

The product grid displays all information correctly.

<u>Actual results</u>:

Inventory data is missing.

## Apply the patch

To apply individual patches, use the following links depending on your deployment method:

* Adobe Commerce or Magento Open Source on-premises: [Software Update Guide > Apply Patches](https://devdocs.magento.com/guides/v2.4/comp-mgr/patching/mqp.html) in our developer documentation.
* Adobe Commerce on cloud infrastructure: [Upgrades and Patches > Apply Patches](https://devdocs.magento.com/cloud/project/project-patch.html) in our developer documentation.

## Related reading

To learn more about Quality Patches Tool, refer to:

* [Quality Patches Tool released: a new tool to self-serve quality patches](https://support.magento.com/hc/en-us/articles/360047139492) in our support knowledge base.
* [Check if patch is available for your Adobe Commerce issue using Quality Patches Tool](https://support.magento.com/hc/en-us/articles/360047125252) in our support knowledge base.

For info about other patches available in QPT, refer to [Patches available in QPT](https://devdocs.magento.com/quality-patches/tool.html#patch-grid) in our developer documentation.