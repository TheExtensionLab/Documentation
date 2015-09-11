---
layout: page
title: Create a dropdown
date: 2015-11-09 11:04:00
category: mega-menu
order: 14
---

Each category should now have two new tabs under Magento Admin > Catalog > Manage Categories as below.

![New Tabs](../assets/images/mega-menu/new-tabs.jpg "New Tabs")

***MegaMenu Settings***

This section controls 3 main things:

* Position of the dropdown
* Type of top level link used
* Alternate name - for use only in the menu.

Note: For a dropdown to display it must first have some content in the content section.

***MegaMenu Content***

This is where you can input the content that you would like to display in the dropdown.

There are two main fields:

* Section X Columns (How many columns should this section take up?)
* Section X Content (The content of this section)

These two fields are however repeated 7 times by default meaning you can set the column width for each section (which uses a grid system) and enter the content to manage the layout directly from the admin.

For example:

You could select:

24 of 24 columns for the first item.
8 of 24 columns (one third) for the second thrid and fouth items.

And you would end up with something like this:

![Basic Layout Example](../assets/images/mega-menu/basic-layout-example.jpg "Basic Layout Example")

***What can I put in the Content Section?***

Section X Content is a WYSIWYG editor and anything you can out in a CMS Page you can enter in here so:

* Widgets
* Static Block Links
* Images
* Raw Html

***HOWEVER We strongly recommend where possible using our "Widgets" prefixed with "MegaMenu -"*** This is because our widgets will be pre-processed to load all the data required in one go.

![MegaMenu Widgets](../assets/images/mega-menu/megamenu-widgets.jpg "MegaMenu Widgets")

For example if you have 3 sets of featured products in your Menu with Ids 22,33,44 - 32,46,13 and 45,53,34.
Usually this would require 3 collections (or worse 9 ->load calls), however our widgets would load all products in one collection saving resources.
Within our widgets all calls to categories will also use the already loaded menu tree saving the need to call the database once again.

[If you are un-familiar with Widgets please see this short gif animation](/mega-menu/using-a-widget-demo.html)

For now you can just enter text into the content boxes to see how they work, once that is OK you may want to checkout one of the following examples:

* Creating a Menu List Block
* Creating a Featured Category Block
* Creating a Featured Product Block/List
* Creating a Shop By Attribute Block
* Add a top level link that is not a category (e.g home-page link)