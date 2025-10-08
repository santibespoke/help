---
coverY: 0
---

# Ecommerce Integration

{% embed url="https://www.youtube.com/watch?v=hpTmNybVbbQ&ab_channel=BespokeFactory" %}
Promo Video
{% endembed %}

## Sell Pre-Designed Styles

If you have an existing ecommerce, you can add pre-designed styles to your shop and start selling them online as "closed" products.

You can choose any style from our "Get Inspired" gallery to take advantage of our ready-to-use product images and lifestyle pictures, or create your own styles from scratch.&#x20;

When a customer purchases one of these products though your ecommerce, item data and buyer information is transferred to our systems, and the new order will appear on your backoffice production panel.

We then take care of the production and shipping to your customer's adress on your behalf.

{% embed url="https://i.gyazo.com/3726445d7a7cb36b3b900b68f6ab58fb.gif" %}
Example of how your ecommerce may look
{% endembed %}

## Video Walkthrough

The "Guided Walkthrough" video provides step-by-step instructions on setting up your ecommerce and integrating our designs seamlessly. You'll learn how to navigate your backoffice production panel, select pre-designed styles from our "Get Inspired" gallery, and upload them onto your platform.&#x20;

This walkthrough ensures that your ecommerce site is not only visually appealing but also operationally efficient, allowing you to start selling quickly and effectively.

{% embed url="https://www.youtube.com/watch?v=9R5O5FdE8xI&ab_channel=BespokeFactory" %}
Guided Walkthrough
{% endembed %}

## Requisites

Please, make sure you comply with all requisites below, before moving forward.

* [ ] Have a working account with us with admin credentials for your platform.
* [ ] [Set up shipping, billing and contact information ](broken-reference)on your backoffice.
* [ ] [Set up retail prices](broken-reference) and currency for all styles on your backoffice.
* [ ] Have an working e-commerce platform (Woocommerce, Shopify or Prestashop)
* [ ] Have your e-commerce integrated with our platform with our integration plugin (one-time fixed cost). [Contact us](../get-help/contact-us.md#need-feedback-create-a-support-request).
* [ ] Adapt your ecommerce installation and theme to allow [external / affiliate products](ecommerce-integration.md#external-affiliate-products).

## Requisite: External / Affiliate Products

{% hint style="danger" %}
This is a technical requirement for Shopify & Prestashop, in order to start selling pre-designed styles. We suggest these modifications to be carried out by an expert
{% endhint %}

External / affiliate products are stored and displayed on your ecommerce, just like standard products. However, instead of a standard "Buy Now" button that adds the item to the cart (as you would expect), their "Buy Now" button is an actual link, which simply loads a custom BUY URL when clicked. The BUY URL is stored on the product itself.

So, when a customer clicks on the "Buy Now" or "Add to Cart" button of one of these external products, the browser is redirected to the custom BUY URL we defined in the product. In our case the BUY URL will load the size selection step inside your ecommerce (iframe).

When the user has finished selecting sizes, it will click on our "Add to Cart" button, which will behave as a standard add-to-cart button: adds the product to the cart and redirects usert to the cart page.

If you use **Woocommerce** there are no additional requisites. **Woocommerce** natively supports external / affiliate products.

On the other side, **Shopify** and **Prestashop** do not support external or affiliate products by default.  A development is required on your side to adapt your installation and theme.

1. We will provide you with a "Buy URL" for each design. You need to find a way to store the "Buy URL" on the product. For example, you can use [Metafields](https://help.shopify.com/en/manual/metafields) for Shopify.
2. Modify your theme to replace any native "Add to Cart" button with the "Buy URL"  stored on the product.

We suggest this process to be carried out by your development team, or hire a web developer for this purpose.&#x20;

Alternatively, you may want to take a look at paid plugins / modules for Shopify and Prestashop that add the same functionality to your shop (affiliate / external products). For instance:

[https://apps.shopify.com/external-affiliate-product-links](https://apps.shopify.com/external-affiliate-product-links)

Note that we don't have any relationship with the above software.

## Choose from our GI gallery

We provide our customers with hundreds of pre-designed styles (Standard MTO, [Fast Lane MTO](../production/pricing-and-production-methods/fast-lane.md) and [48h Rush](../production/pricing-and-production-methods/48h-rush-production.md) production methods) through our [Get Inspired](../admin-backoffice/designing-tools-and-galleries/get-inspired-gallery.md) gallery.

These items already have product images, lifestyle pictures and descriptions, which are ready to be used on your ecommerce!

Select any Get Inspired item and click on “Export to E-commerce” link to open the export panel.&#x20;

{% embed url="https://i.gyazo.com/d790b889342fc15d5a38debcb0216d8e.gif" %}

Here, you will be able to download product images and get all urls and code snippets required to add the item to your ecommerce.&#x20;

Below is a brief explanation of what the fields are and how they work:

* **Buy URL / Add to Cart Link:** this is the main link that should replace the standard "Buy Now" or "Add to Cart" button on your ecommerce. Clicking on this link will lead the customer to the size selection step (iframe) inside your ecommerce. This is managed by our integration plugin.
* **Customize Link / URL (optional):** this link will show the 3D Designing Tool and load the current design. You can add this link anywhere on the product page to allow customers to further personalize the style.
* **Images (optional):** items in our GI gallery have a set of product images and lifestyle pictures ready to be used. You can download them from our gallery and upload as product images in your ecommerce.
* **Description (optional):** we also provide a short description and material information on each Get Inspired item, so you can also add it to your product description or use it as a starting point to create your own ones.
* **Available Sizes Widget Code (optional):** it's an iframe widget that you can embed anywhere on your product page to get a preview of the sizes that are currently available for this style.
  * By default, the widget shows available sizes in each scale. You can use the parameter "scale" to show the sizes in just one specific scale. For example "\&scale=EU"
  * For Standard MTO items the widget will show all the sizes on which the style can be produced in. For [Fastlane](../production/pricing-and-production-methods/48h-rush-production.md) and [48h Rush](../production/pricing-and-production-methods/48h-rush-production.md) items, the widget will show the actual sizes in stock at the moment. Sizes that are not available will be shown disabled. If no sizes are available at all the widget will read "Sorry, this style is not available".

This is an example of how the product page of your ecommerce may look. Take a look at our live [ecommerce demo](https://wordpress-306597-2766026.cloudwaysapps.com/) we built on woocommerce, with a few SKUs added as an example.

<figure><img src="../.gitbook/assets/example (1).jpg" alt=""><figcaption><p>Example Ecommerce</p></figcaption></figure>

## Create a product on your e-commerce

{% hint style="info" %}
Depending on your ecommerce, product creation might be slightly different. We suggest this process to be carried out by your tech team
{% endhint %}

For each style you need to create a product on your ecommerce, and fill it with all the information and images you can find on the Get-Inspired item export panel (see previous section).&#x20;

Instructions for Woocommerce: [https://woocommerce.com/document/managing-products/#adding-an-external-affiliate-product](https://woocommerce.com/document/managing-products/#adding-an-external-affiliate-product)

Instructions for Shopify: [https://help.shopify.com/en/manual/products/add-update-products](https://help.shopify.com/en/manual/products/add-update-products)

Instructions for Prestashop: [https://doc.prestashop.com/display/PS17/Managing+Products](https://doc.prestashop.com/display/PS17/Managing+Products)

## Batch export CSV

We provide you with a json / csv endpoint with updated information of all Get-Inspired items available in our platform at the moment.

You can use this CSV to batch upload all the items to your ecommerce programmatically.

<figure><img src="../.gitbook/assets/Captura de pantalla 2024-12-10 a las 18.24.42.jpg" alt=""><figcaption><p>Example csv file</p></figcaption></figure>

{% hint style="warning" %}
Import & sync your ecommerce database with our csv endpoint will require custom development on your side. We suggest all development to be carried by an expert
{% endhint %}

Also, you can also use the endpoint to create a sync mechanism between your ecommerce and our platform, to automatically keep all items in the store updated and in-sync with our platform.

Please, [contact us](../get-help/contact-us.md) for more information.

## Sell a Custom Style

You can design your own style from scratch, and add these styles as purchasable pre-designed items in your ecommerce, just like you can do it with our Get-Inspired items.

First, design any style you want using your 3D Designing Tool, and click on "Order". You must be logged in as Admin before continuing.&#x20;

On the first step of the checkout process there will be a banner where you copy both **Buy URL** and **Customize URL** for this specific style.

![](<../.gitbook/assets/Captura de pantalla 2022-02-10 a las 11.29.09 (1).jpg>)

Use these codes in the same way to add the products to your ecommerce.&#x20;

If you need product images for your ecommerce, you can launch the style to production, as usual, and ask us to take pictures (e-commerce photography service). We will produce the order and shoot white-background studio pictures for you, before shipping the item.
