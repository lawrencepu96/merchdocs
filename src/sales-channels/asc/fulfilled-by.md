---
title: Fulfilled By
redirect_from:
  - /sales-channels/amazon/ob-fulfilled-by.html
---

Fulfilled By settings are part of your store's listing settings. Listing settings are accessed from the [store's dashboard]({% link sales-channels/asc/amazon-store-dashboard.md %}).

Fulfilled By settings define who fulfills (or ships) orders. If all of your orders are fulfilled using one method, choose between merchant (you) or Amazon. If you plan on fulfilling orders from your locations and using Amazon, we recommend using the third option and configuring a Magento product attribute.

- **Fulfilled by Merchant** - Choose when you, the merchant, will fulfill all orders. When an order is placed, inventory will be deducted from your Magento catalog.

- **Fulfilled by Amazon** - Choose when Amazon will fulfill all orders. When chosen, product inventory is not deducted from your Magento catalog when an order is placed. Inventory stock for Amazon fulfilled orders is stored and deducted from their warehouses. Before assigning this option, you must verify in your Amazon Seller Central account that your products are eligible for FBA fulfillment. FBA inventory is directly managed through your Amazon Seller Central Account. With this fulfillment method, Amazon Sales Channel does not share quantity updates between Magento and Amazon. Therefore, not all of the marketing tools described in the Quantity Settings will be available to you in Amazon Sales Channel.

- **Assign Fulfilled By Using Magento Product Attribute** - If your products may be fulfilled by you and Amazon, you may want to create a Magento product attribute with values for Fulfilled By Merchant and Fulfilled by Amazon. Setting this value per product indicates who fulfills the orders.

The fulfillment method is a regional attribute, and based on the Amazon Marketplace option selected during [store integration]({% link sales-channels/asc/store-integration.md %}). When a change is made, the change will affect all Amazon listings that share that Amazon Seller SKU in your Amazon stores that sell in the same region (as defined during the store's integration). This means that a change to a shared Amazon Seller SKU in the North America region will not affect your Amazon stores with a region set for a different region (as defined during the store's integration).

## Configure Fulfilled By settings

1. Expand **Fulfilled By**.

1. For the **Product Fulfilled By**, choose who fulfills (ships) the order:

    - **Fulfilled by Merchant** - Merchant fulfills order.

    - **Fulfilled by Amazon** - Amazon warehouse fulfills order.

    - **Assign Fulfilled By Using Magento Product Attribute** - A Magento attribute indicates who fulfills the order per product. If selected, then select the Magento attribute for **Fulfilled by Attribute**.

![]({% link sales-channels/asc/assets/amazon-fulfilled-by.png %}){: .zoom}
_Fulfilled By_

|Field|Description|
|--- |--- |
|Product Fulfilled By|Options:<br/>**Fulfilled by Merchant** - (FBM) Select this if you fulfill the orders. When an order is placed, inventory will be deducted from your Magento catalog. When a new product is created, the fulfillment method of Merchant Fulfilled will be assigned.<br/>**Fulfilled by Amazon** - (FBA) Select this if Amazon fulfills the orders. With this fulfillment method, product inventory will not be deducted from your Magento catalog when an order is placed. When a new product is created it will be created with Fulfilled by Amazon (FBA) as the fulfillment type. You will need to ensure that your products are eligible for FBA fulfillment within your Amazon Seller Central account. FBA inventory is also directly managed through your Amazon Seller Central account. With this fulfillment method quantity updates are not pushed out relative to your Magento catalog, so you will be unable to use some of the marketing tools described in the Quantity Settings.<br/>**Assign Fulfilled By Using Magento Product Attribute** - Select this if you have an existing Magento attribute that determines if it is fulfilled by the merchant or fulfilled by Amazon. When chosen, **Fulfilled by Attribute** enables. |
|Fulfilled By Attribute|Select the Magento attribute used to determine the fulfillment method.<br/><br/>For example, if the attribute is Fulfilled By and you select the respective attribute value to denote if it is Fulfilled By Merchant or Fulfilled By Amazon (FBA), when a new product is created it will be created with FBA as the fulfillment type. As a merchant, you will need to ensure that your products are eligible for FBA fulfillment within your Amazon Seller Central account. FBA inventory is also directly managed through your Amazon Seller Account.<br/><br/>Options in this list depend on the attributes you set up for your Amazon products. |