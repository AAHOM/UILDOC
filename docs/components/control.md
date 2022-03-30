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

**Usage**

*collectionControl(Selector, Collection Slug, Display Type, Attributes)*

**Parameters:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td><em>Selector</em></td>
      <td>Required.<br>jQuery selector identification where the resulting html code will be generated.</td>
    </tr>
  </tbody>
</table>


**Example code block for control**

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