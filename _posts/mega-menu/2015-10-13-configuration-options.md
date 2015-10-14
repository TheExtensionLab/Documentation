---
layout: page
title: General Configuration Options
date: 2015-11-09 11:04:00
category: mega-menu
order: 25
---

This extension comes with a few general configuration options that can be located at Magento Admin > System > Configuration > Catalog > Category Top Navigation.

***Serial Key***: Hopefully self explanatory. Your serial key can be found in My Accounts > Serial Keys once this extension has been purchased on http://www.theextensionlab.com

***Include Responsive Styles***: Responsive css styles (css for mobiles and tablets in this case) are included by default, if your site is not responsive you may wish to turn this off.

***Maximal Depth***: This sets how deeps down the category tree Magento should load. And in the case of this extension is used for prefetching of categories to be shown later in the dropdowns. 0 will load all categories, 1 just the first level 2 the level under than and so on.

We recommend setting this to the lowest possible value (not including 0) bearing in mind that any categories shown via the MegaMenu widgets within the dropdowns will need to be equal or less than the level you set. This helps Magento load times as it will not load unused category levels.