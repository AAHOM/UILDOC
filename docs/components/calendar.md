---
layout: default
title: Calendars <span class="new">(Updated)</span>
parent: Components 
nav_order: 2
---

### Calendar of Events

The calendar custom function grabs data from the reference-data blog "Calendars"

**Used On Pages**

*About Us -> Calendars*

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
      <td>No defined collection is needed, leave blank.</td>
    </tr>
    <tr>
      <td><em>Display Type</em></td>
      <td>Required.<br>Identifies the display type requested.  For calendars must be "calendars".  These are case sensitive parameters. </td>
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
      <td>ActiveTab</td>
      <td>Optional.
        <ul>
          <li>0=All museums (Default)</li>
          <li>1=Ann Arbor Hands On</li>
          <li>2=Leslie Science</li>
          <li>3=Yankee Air Museum</li>
          <li>4=Challenger Learning center</li>
        </ul>
     </td>
    </tr>
    <tr>
      <td>single</td>
      <td></td>
    </tr>
    <tr>
      <td><em>openfirst</em></td>
      <td>Optional.<br>
      Determins if the first accordian group is initially expanded or not
        <ul>
          <li>True=Initially collapsed</li>
          <li>False=Initially expanded (default)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Collapasble</td>
      <td>Optional.
        <ul>
          <li>True=Can be collapsed or expanded (Default)</li>
          <li>False=Not collapsable</li><li>true=Can be collapsed or expanded (Default)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><em>Collapsed</em></td>
      <td>Optional.<br>
      Collapsable must be set to true, otherwise this paramter is ignored.
        <ul>
          <li>True=Initially collapsed</li>
          <li>False=Initially expanded (default)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>showPrint</td>
      <td></td>
    </tr>
    <tr>
      <td>title</td>
      <td>The title that will be displayed if collapsable</td>
    </tr>
    <tr>
      <td>showName</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

**Example code block for control**

```
<script>
$(document).ready(function() {
  collectionControl(
    '#calendarsOut',
    '',
    'calendars',
    {activetab: 1,
     single: false,
     openFirst: false,
     collapsable: false,
     collapsed: false,
     title: "View Calendars",
     showPrint: false,
     showTabs: false,
     showTitle: false,
     showName: false,
     showNav: true,
     showDate: true,
     showTz: true,
     mode: "MONTH",
     showCalendars: false}
  );
})
</script>
<div id="calendarsOut"></div>
```

**Reference Data**

*reference-data blog: Donor Wall (code block)*

**Overrides:**

You can dynamically override *ActiveTab* by adding a parameter to the linking url as:

```
?tab=n  (where n is a number from 0-4, see ActiveTab below)
```


**Return Value:**

None

**Google Spreadsheet:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Detail</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>Owner</td>
      <td>aahom220@gmail.com</td>
    </tr>
    <tr>
      <td>File Name</td>
      <td>Google Calendars</td>
    </tr>
    <tr>
      <td>Folder</td>
      <td><a href="https://drive.google.com/drive/folders/1YaVLSr9quHsbMDChBrlZUjpI_ZeG0cG-" target="_blank">UIL_Web_Site_Docs</a></td>
    </tr>
    <tr>
      <td>Link</td>
      <td><a href="https://docs.google.com/spreadsheets/d/1i5EjZCpxI4UnvXyMYXCLyLP9tSCNt0PZYemaU6f6XtU/edit#gid=0" target="_blank">Google Calendar Spreadsheet</a></td>
    </tr>
    <tr>
      <td>ID</td>
      <td>1i5EjZCpxI4UnvXyMYXCLyLP9tSCNt0PZYemaU6f6XtU</td>
    </tr>
    <tr>
      <td>Sheet Name</td>
      <td>Calendars</td>
    </tr>
  </tbody>
</table>

**Spreadsheet Fields**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
    <td style="width:20px">Column</td>
    <td style="width:120px">Label</td>
    <td>Description</td>
    </tr>
    <tr>
    <td>A</td>
    <td>Order</td>
    <td>Order calendars should be displayed</td>
  </tr>
  <tr>
    <td>B</td>
    <td>Museum</td>
    <td>Museum code, aahom, lesli etc</td>
  </tr>
  <tr>
    <td>C</td>
    <td>Name</td>
    <td>Short name assoiciated with museum</td>
  </tr>
  <tr>
    <td>D</td>
    <td>Hide</td>
    <td>Checked or Yes=Hide this museum when displaying calendars.</td>
    </tr>
    <tr>
    <td>E</td>
    <td>Title</td>
    <td>Long name associated with museum</td>
    </tr>
    <tr>
    <td>F</td>
    <td>iFrame</td>
    <td>The html iFrame code to display this calendar in monthly display.</td>
  </tr>
    <tr>
    <td>G</td>
    <td>After</td>
    <td>Text to display as footer after calendar</td>
    </tr>
  </tbody>
</table>

**Calendar desktop view**

![Alt Calendar Desktop](../../assets/images/calendar.jpg "Calendar Desktop")

**Calendar mobile view**

![Alt Calendar Mobile](../../assets/images/calendar_mobile.jpg "Calendar Mobile")