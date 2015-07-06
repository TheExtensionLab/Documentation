---
layout: page
title: Installation
date: 2015-01-18 21:04:00
category: trustpilot-feed
order: 10
---

Once purchased you will be provided with 2 download methods in your ```My Account > Downloadable Products``` Page, Direct download and Github.

***Installation Via Direct download***

1. Unzip the files
2. Check Compilation status and disable Compilation if it is enabled (Magento Admin > System > Tools > Compilation)
3. Copy the files from the package into your Magento directory
4. Clear your Magento Cache. (```Magento Admin > System > Cache Management > Select "Flush Cache Storage"```)
5. Your extension should now be installed. And just requires configuration details on which can be [found here](/kit-products/configuration.html)

***Installation via Modman/Github***

Via Modman

```modman clone https://github.com/TheExtensionLab/Kitproducts```

Via Composer

Add ```"theextensionlab/kitproducts": "~1.0.0"``` to your required section and add the github repo as a source
repositorie by adding it to the composer.json repositories array``{"type": "vcs", "url": "https://github.com/TheExtensionLab/CustomContactUrl.git"}```

Once installed you will need to configure the extension and add your serial key details on how to do this can be configuration details on which can be [found here](/kit-products/configuration.html).