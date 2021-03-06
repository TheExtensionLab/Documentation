---
layout: page
title: Configuration
date: 2015-01-18 16:50:00
category: status-colors
order: 1
---

***Changing order status colors***

You can assign any color to a status from ```Magento Admin > System > Order Statuses```. A new field called Status Color will have been added to both the Edit and New Order Status pages.

Once on ```Magento Admin > System > Order Statuses``` simply select the row of the status you could like to change click the "Status Color" Field select the color you would like to use and hit Save Status, if the save was successful you should then see a success message "The order status has been saved." and the new color will be demonstrated in the Status Color column of the status grid.

![Select a status color](../assets/images/select-a-status-color.png "Select a status color")

***Changing the default Status Color***

To make it easy to see when the installation was successful we added a default Status Colour, if you want to change or remove that you can do so from ```Magento Admin > System > System Configuration > Advanced > Admin > Order Grid```. You should then see a Default Status Color field simply update that as needed.

***How do I highlight the whole row rather than just the status within that row?***

If you would like to highlight the whole row on the order grid rather than just the status there is a setting for that. Navigate to the new Order Grid settings section under ```Magento Admin > System > System Configuration > Advanced > Admin > Order Grid```, change ```Color Whole Row``` to yes and hit save config. The next time you visit the sale order grid page the whole row should now be colored in.

![Row Style option](../assets/images/status-display-style.png "Row Style option")
