---
layout: default
title: SubMenu List <span class="new">(06/06/22)</span>
parent: Reference
nav_order: 4
---

# SubMenu List

Menu bar for sub-menu items.  These are found on the "Learn" pages to help navigation between learn pages.  On mobile devices the menu is an wrapped in an accordion and compressed by default to save some space.  Content for submenu bar is in a code block
of the SubMenu List reference-data blog.

To edit SubMenus, navigate to Reference-data -> SubMenu List.  Open the first code
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
    <td>Menu</td>
    <td>This is the menu group for which buttons will be grouped together.</td>
  </tr>
  <tr>
    <td>C</td>
    <td>Label</td>
    <td>The label string for the button.</ul>
    </td>
  </tr>
  <tr>
    <td>D</td>
    <td>Slug</td>
    <td>The page slug used for the button link.</ul>
    </td>
  </tr>
  </tbody>
</table>

![Alt Editing Submenu](../../assets/images/refsubmenu.jpg "Editing SubMenu"){: .theImage}

