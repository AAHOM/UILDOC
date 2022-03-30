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
      <td>Required.<br>jQuery selector identification where the resulting html code will be generated.  Note that the selector must be unique on the page.</td>
    </tr>
    <tr>
      <td><em>Collection Slug</em></td>
      <td>Required.<br>This is the internal slug (key) assigned to the collection.  You can find this by looking going to the page settings -> General, under URL SLUG.</td>
    </tr>
    <tr>
      <td><em>Display Type</em></td>
      <td>Required.<br>Identifies the display type requested.  Must be one of "grid", "carousel", "team" or "flexboxes".  These are case sensitive parameters. </td>
    </tr>
    <tr>
      <td><em>Attributes</em></td>
      <td>Optional.<br>Identifies parameters to override default values.  The parameters are passed in a object array of key/value pairs.  Each display type has different default values as described below. </td>
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

**Example Team Members code block**

This code block can be found on the *About Us -> People page*.   It will display team members from the **Team Members** blog with the slug name "**team-members**", using the display type "**team**".  All additional attributes are turned off so categories and filter checkboxes are not shown, as an example. 

```
<script>
$(document).ready(function() {
  collectionControl(
    '#teamContainer',
    'team-members',
    'team', 
    {filter: false, 
     showcount: false,
     groups: '',
     showcats: false,
     findcats: '',
     dots: true}
  );
})
</script>
<div id="teamContainer"></div>
```