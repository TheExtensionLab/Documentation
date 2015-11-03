---
layout: page
title: Installation
date: 2015-01-18 21:04:00
category: mega-menu
order: 10
---

Once purchased you will be provided with 2 download methods in your ```My Account > Downloadable Products``` Page, Direct download or Github.

***Installation Via Direct download***

1. Unzip the files
2. Check Compilation status and disable Compilation if it is enabled (Magento Admin > System > Tools > Compilation)
3. Copy the files from the package into your Magento directory
4. Clear your Magento Cache. (```Magento Admin > System > Cache Management > Select "Flush Cache Storage"```)
5. Your extension should now be installed. And just requires configuration details on which can be [found here](/mega-menu/configuration.html)

***Installation via Composer/Modman***

Via Composer (Reccomended over Modman if possible)

Add ```"theextensionlab/megamenu": "~1.0"``` to your required section and add the github repo as a source
repository by adding it to the composer.json repositories array. Since composer wont resolve repositories recursively we also need to add the source of two small dependencies.

```
          {
              "type": "vcs",
              "url": "https://github.com/TheExtensionLab/MegaMenu.git"
          },
          {
              "type": "vcs",
              "url": "https://github.com/TheExtensionLab/TinyMceConfig.git"
          },
          {
              "type": "vcs",
              "url": "https://github.com/TheExtensionLab/WidgetImage.git"
          }
```

Once installed you will need to configure the extension and add your serial key details on how to do this can be configuration details on which can be [found here](/mega-menu/configuration.html).

Via Modman

This extension has 2 other extension dependencies so you will need to install all 3 via modman


```modman clone https://github.com/TheExtensionLab/MegaMenu.git```

```modman clone https://github.com/TheExtensionLab/TinyMceConfig.git```

```modman clone https://github.com/TheExtensionLab/WidgetImage.git```