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

This is where you can input the content you’d like to display in the dropdown.

Each dropdown is made up of “sections". Each section is simply a block of code or content that you would like to display within a certain section of the dropdown block.

By default you can have up to 7 sections in a dropdown, each has two options:

1. Section Width - Width of this section - Based on a grid system, e.g 12 of 24 = 50%
2. Section Content - Here you can enter widgets, code, or text to display within that section.

For example:

You could configure you dropdowns like this.

* Section 1 - 24 of 24 columns (full width)
* Section 2 - 8 of 24 columns (one third)
* Section 3 - 8 of 24 columns (one third)
* Section 4 - 8 of 24 columns (one third)
* Section 5 - 12 of 24 columns (one half)
* Section 6 - 12 of 24 columns (one half)

As long as you enter some content into each sections content section you would end up with something like this:

![Basic Layout Example](../assets/images/mega-menu/grid-layout-example.jpg "Basic Layout Example")


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