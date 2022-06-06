---
layout: default
title: Categories <span class="new">(06/05/22)</span>
parent: Reference
nav_order: 3
---

# Reference Data - Categories

This list of category names and groupings are used internally in various places.  Specifically, they are used in filtering grid displays.   However the use is not
limited to grids.  The category data is saved in a page code block in CSV format.

To edit categories, navigate to Reference-data -> Categories.  Open the first code
block and edit the content as CSV data.

**CSV Fields**

<table class="ws-table-all notranslate">
  <tbody>
    <tr class="tableTop">
    <td style="width:20px">Column</td>
    <td style="width:120px">Label</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>A</td>
    <td>Group</td>
    <td>The group name given here must match a group name from the Category Groups CSV
      file, column A.
     </td>
  </tr>
  <tr>
    <td>B</td>
    <td>Category</td>
    <td>Category Name.  This name should match blog category names where given
    in blog or event items</td>
  </tr>
  <tr>
    <td>C</td>
    <td>Hide YesNo</td>
    <td>Setting to Yes will hide his field.  The field will be ignored.
    valid values are:
      <ul><li>Yes</li>
        <li>No</li>
        <li>or blank (no value)</li>
      </ul>
    </td></td>
  </tr>
  </tbody>
</table>

![Alt Categories](../../assets/images/referencecategories.jpg "Categories"){: .theImage}
