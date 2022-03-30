---
layout: default
title: Control 
parent: Components 
nav_order: 1
---

### Control

Controls the display of any blog or event collections as one of:

- Slick carousel
- Grid
- Team Members
- Flex Boxes 

**Basic Syntax**

```
<script>
$(document).ready(function() {
  collectionControl(
    '#demo2',
    'outreach-1',
    'grid',
    {filter: true, 
     groups: 'grades,outreach',
     showcats: true,
     showcount: true,
     dots: false}
  );
})
</script>
<div id="demo2"></div>
``` 