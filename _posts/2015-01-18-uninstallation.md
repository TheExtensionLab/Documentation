---
layout: page
title: Uninstallation
date: 2015-01-18 17:59:00
category: status-colors
order: 100
---

To uninstall this extension you need to run the following SQL after removing the extension files a list of which can be found in the modman file:
```sql
  ALTER TABLE `sales_order_status` DROP `color`;
```