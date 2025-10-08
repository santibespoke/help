---
description: >-
  In this settings page you will be able enable / disable styles, as well as
  stablish retail prices for every style and customization availbale.
---

# Update Prices

## Activate / Deactivate All

These controls allow you to Activate or Deactivate all available styles. Please, note that this operation cannot be undone. To activate / deactivate specific styles, look for their individual controls on the [library](update-prices.md#library) (see below)

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.15.02.jpg>)

## Library Prices

This panel helps you activate, deactivate and assign retail prices to each individual model (and model variation).

{% embed url="https://i.gyazo.com/ad64bce206402494dc99075a987e53a3.gif" %}

### Set Prices

Each row represents a model, for example Derby Shoe, easily identifiable by its thumbnail. Then, for each row (model), you will see a number of black boxes with the name of the variation. On each box there is an active / inactive switch, the wholesale cost information, and editable retail price.&#x20;

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.12.43.jpg>)

Each of these boxes represents a configuration of that model. For example, a Derby Shoe can be offered in different configurations: Blake, Goodyear, Fastlane, Golf, Burnishing, Exotic Skins, or some other variation.&#x20;

These model variations have different manufacturing prices, thus you can assign different retail prices for each of them.

{% hint style="info" %}
Manufacturing costs are shown in EUR. Retail prices are set in the currency of your store. You can change the currency of your store on **Configuration > Data > Retail**
{% endhint %}

The retail price that you assign to each model is the selling price that will be shown to your customers. Remember that this is the base retail price (no taxes or shipping included).

If you update a price and you are using an ecommerce integration, remember that you must also change the retail price of the associated products on your ecommerce.

### Shorcuts

* **Links to model categories**: these are shorcut links that will take you to each category.

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.09.44.jpg>)

* **Men Dress / Available Last**: this feature allows you to Activate / Deactivate the Mens Dress category. It also allows you to Activate / Deactivate certain shoe lasts, all at once.

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.10.59.jpg>)

## Other Costs

These panels allow you to configure other services, extra costs, or add-ons, that your customers may request.

These controls allow you to Activate or Deactivate all available styles. Please, note that this operation cannot be undone

### Group Prices (Art Sole, Beveled Waist, etc)

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.21.13.jpg>)

These are features, add-ons or extra services that can be added to the original item for am extra cost. For example, the Fur Lined Interior on selected styles.&#x20;

On this table you will see each item extra cost (manufacturing price). If you click on the EDIT button you will be able to assign a Retail Price for that item.&#x20;

You can also activate / deactivate an item, and your customers won’t be allowed to use it (it won’t be showed).

Note that if you choose zero as a retail price, no extra cost will be charged to your customers if they use that item or feature in their designs.

### Extra Costs (EEE extra cost)

These are extra manufacturing costs that depend on manufacturing constrains. For example, the associated extra cost for (EEE) triple extra wide goodyear shoes.&#x20;

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.21.54.jpg>)

The list will show all extra cost items. You can click the EDIT button to activate / deactivate the item and assign a retail price, that is, the extra cost that will be shown to your customers.

### Embossed Initials

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.22.13.jpg>)

Initials can be engraved in most of our shoes. You can activate / deactivate this feature, to show or hide this option to your customers.

You can set the retail price (extra cost) that your customers will be charged for this service.&#x20;

For reference, you can also see the manufacturing cost below, that is, the actual wholesale extra cost that you will pay.

### Matching Belt

![](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.22.49.jpg>)

Matching belt is a limited service offered in some specific shoe styles. Using this feature a customer is able to add a matching belt during the checkout process.

On this panel you can activate / deactivate this feature. The price for the matching belt is the same as an actual MTO belt. If you want to change these prices, scroll down to the Belt section of the Library and assign your desired selling prices.

## Price Update Batch Tool

The batch update feature is an advanced tool that allows you to make a variety of operations to the entire catalog of prices, based on the actual retail price of the style, or its manufacturing cost. Use carefully, since this operation will be applied to all your retail prices, or a subset of them. You won’t be able to undo the changes or restore previous prices.

#### **How it works?**

First, decide which price should be used as the base for the computation. The wholesale price, that is, the actual manufacturing cost that you will be paying. Or the retail price, that is, the amount that is currently established as the selling price for your end customers.

#### **Which one should I chose?**

It depends. Use wholesale price to compute retail prices in a way that you always get the same % benefit margin across all styles. On the other side, use retail price if you just want to increase or decrease your current retail prices, which should have been previously stablished.

#### **Update Based on Wholesale Price**

![Batch update based on wholesale price](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.25.19.jpg>)

Using this option, you can set up retail prices in a way that you always get the same percentage (benefit or commission) across all styles, considering the actual manufacturing cost you will have to pay for the production.

* **% Benefit fo MTO**: This is the margin (%) that will be applied to the wholesale price. For example, imagine an item with a wholesale cost of 100 EUR. If you set this option to 80%, retail price will be 180 EUR. Set it to 200% and the retail price would be 300 EUR. Similarly, set it to 0% to assign retail prices to manufacturing costs.
* **Rounding**: Operations which are based on percentages usually result in awkward retail prices, like 238,57 EUR. Use the options below to automatically round up the numbers so they all look aesthetically pleasant and similar. \
  \
  Whole part: A number from 0 to 99. Rounds the all prices to the closer upper number. For example, if the price is 226,XX and you set “0” the price would be 230,XX. If you set “5” the price will be 235,XX. If you set “9” the price will be 229,XX. If you set “10” the price will be 310,XX\
  \
  Decimal part: A number from 0 to 99. Rounds the decimal part to the closer upper number. For example, if the price is XXX,29 and you set “0” the price would be XXX,00. If you set “20” the price will be XXX,20. If you set “50” the price will be “XXX,50”. If you set “99” the price will be “XXX,99”.

Rounding is always required, default values are Whole part (0) + Decimal (0) to ger prices to look like 220.00, 230.00, 240.00.

\
Find below some combinations of whole + decimal parts to help you understand how it works:

<table><thead><tr><th>Operation / Base Retail Price</th><th width="150">200,00</th><th width="150">215,15</th><th width="150">224,46</th><th>237,76</th></tr></thead><tbody><tr><td>Whole (00) + Decimal (00)</td><td>200,00</td><td>220,00</td><td>230,00</td><td>240,00</td></tr><tr><td>Whole (00) + Decimal (50)</td><td>200,50</td><td>220,50</td><td>230,50</td><td>240,50</td></tr><tr><td>Whole (05) + Decimal (00)</td><td>205,00</td><td>225,00</td><td>225,00</td><td>245,00</td></tr><tr><td>Whole (09) + Decimal (99)</td><td>209,99</td><td>219,99</td><td>229,99</td><td>239,99</td></tr><tr><td>Whole (10) + Decimal (00)</td><td>210,00</td><td>310,00</td><td>310,00</td><td>310,00</td></tr><tr><td></td><td></td><td></td><td></td><td></td></tr></tbody></table>

**Update Based on Current Retail Price**

![Batch update based on current retail price](<../../.gitbook/assets/Captura de pantalla 2022-05-23 a las 15.25.07.jpg>)

Using this option you will be able to increase or decrease current retail prices, all at once. That is, you will be using the retail prices that were already stablished, and simply increase or decrease them. There are a few options to choose from, see below:

* **Amount:** This is the specific amount (or percentage number) that is going to be used for the operations.
* **Add or Subtract**: Choose if you want to increase or decrease the current retail prices
* **Fixed or Percentage:** Choose either you want to use the first field as a fixed amount or a percentage over the current retal prices.
* **Model Category:** Choose “All Categories” to update all styles, or select the specific category being updated.

See some examples below:

* Amount (50) + Add + Fixed: This will add 50 EUR (or the currency being used) to current retail prices. An item that has a retail price of 200 EUR, will now be selling for 250 EUR
* Amount (10) + Add + Percentage: This will add a 10% to current retail prices. An item that has a retail price of 200 EUR, will now be selling for 220 EUR
* Amount (20) + Subtract + Percentage: This will decrease current retail prices by 20%. An item that has a retail price of 200 EUR, will now be selling for 160 EUR

Please, note that retail prices will be replaced after you click on Update Prices. This operation cannot be undone.
