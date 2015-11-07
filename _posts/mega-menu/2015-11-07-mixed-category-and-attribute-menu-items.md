---
layout: page
title: Mixed Category and Attribute Menu Items
date: 2015-11-07 22:45:00
category: mega-menu
order: 25
---

Sometimes it can be usefull to mix category links and shop by filter links in the same list block like below:

```
    List Title
    menu entry 1 (this should be a link to a category)
    menu entry 2 (this should be a link to an attribute / filter)
    menu entry 3 (this should be a link to a category)
    menu entry 4 (this should be a link to a category)
    menu entry 5 (this should be a link to an attribute / filter)

```

This can be achieved using our li-only widget templates and a little extra wrapping html.

You will need to add the wrapping html manually to your MegaMenu section input textarea as below then add category widget and shop by attribute widgets within this
and simply select the "Li Only List" template for each widget.

```
    <div class="list-block megamenu-list-block">
        <ul>
            {{ "{{ category widget " }}}}
            {{ "{{ shop by attribute widget " }}}}
            {{ "{{ category widget " }}}}
            {{ "{{ shop by attribute widget " }}}}
        </ul>
    </div>
```



***Note:*** You can select this "Li Only Template" at the bottom the of widget template as per the image below.
![Widget template example](../assets/images/mega-menu/widget-template-example.jpg "Widget template example")