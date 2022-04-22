---
layout: default
title: Flip Boxes <span class="new">(4/22/22)</span>
parent: Components
nav_order: 4
---

### Flip Boxes

Home page flip boxes for Visit, Learn and Support.

**Used On Pages**

*Home*

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
      <td>flex-boxes</td>
    </tr>
    <tr>
      <td><em>Display Type</em></td>
      <td>Required.<br>Identifies the display type requested.  For Flex Boxes must be "flexboxes".  These are case sensitive parameters. </td>
    </tr>
    <tr>
      <td><em>Attributes</em></td>
      <td>Optional.<br>Identifies parameters to override default values.  The parameters are passed in a object array of key/value pairs.  Each display type has different default values as described below. </td>
    </tr>
  </tbody>
</table>

**Attributes:**

<table class="ws-table-all notranslate">
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Attribute</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>FindCats</td>
      <td>Optional.
        This is a comma delimeted list of categories.  The blog entry must
        have one or more of these categories in order to be includede.   If this attreibute
        is not defined, then all blog entries from the defined blog will be included.
      </td>
    </tr>
  </tbody>
</table>

**Example code block for control**

```
<script>
$(document).ready(function() {
  collectionControl(
    '#flexBoxes',
    'flex-boxes',
    'flexboxes',
     {findcats: "Home"}
  );
})
</script>
<div id="flexBoxes"></div>
```

**Reference Blog**

*Flex Boxes*


**Example Screenshot**

![Alt Home Page Flip Boxes](../../assets/images/flip_boxes.jpg "Home Page Flip Boxes")