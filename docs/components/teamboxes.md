---
layout: default
title: Team Members <span class="new">(Updated)</span>
parent: Components
nav_order: 4
---

### Team Members

The team_members custom function grabs data from a Google spreadsheet (teams) and dynamically builds a list of all team members, ordered by last name, first name.  Each team member is displayed in a separate flex box with name and title.  Hovering over team member displays the members profile, if provided.   Clicking on the team member displays the details in a modal box.  It uses the spreadsheet information to get the associated team member information. 

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for team members**
```
<script>
$( document ).ready(function() {
    // SelectorID
    do_team_members('#teamContainer'); 
});
</script>
<div id="teamContainer"></div>
``` 

**Overrides:**

None


**Usage:**

*do_team_members(SelectorID)*

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
      <td>Team Members</td>
    </tr>
    <tr>
      <td>Folder</td>
      <td><a href="https://drive.google.com/drive/folders/1YaVLSr9quHsbMDChBrlZUjpI_ZeG0cG-" target="_blank">UIL_Web_Site_Docs</a></td>
    </tr>
    <tr>
      <td>Link</td>
      <td><a href="https://docs.google.com/spreadsheets/d/1hiPd3cJMf_JOr3Z4RnR3XA6-Z927OSJhxJJgYXix448/edit#gid=0" target="_blank">Google Calendar Spreadsheet</a></td>
    </tr>
    <tr>
      <td>ID</td>
      <td>1hiPd3cJMf_JOr3Z4RnR3XA6-Z927OSJhxJJgYXix448</td>
    </tr>
    <tr>
      <td>Sheet Name</td>
      <td>Members</td>
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
    <td>First Name</td>
    <td>Team member first name</td>
  </tr>
  <tr>
    <td>B</td>
    <td>Last Name</td>
    <td>Team member last name</td>
  </tr>
  <tr>
    <td>C</td>
    <td>Organization</td>
    <td>Organization code, aahom, leslie, etc.  This is currently not used.</td>
  </tr>
  <tr>
    <td>D</td>
    <td>Unused</td>
    <td>Extra field not used</td>
    </tr>
    <tr>
    <td>E</td>
    <td>Title</td>
    <td>Position or responsibility in organization</td>
    </tr>
    <tr>
    <td>F</td>
    <td>Hide</td>
    <td>If = Yes, Hide the team member from display.</td>
  </tr>
    <tr>
    <td>G</td>
    <td>Image URL</td>
    <td>Full URL to the team member image</td>
    </tr>
    <tr>
    <td>G</td>
    <td>Bio Excerpt</td>
    <td>Team members bio</td>
    </tr>
  </tbody>
</table>

**Example Screenshot**

![Alt Team Members](../../assets/images/team_members.jpg "Team Members")

**Team member detail**

![Alt Team Member Detail](../../assets/images/team_member_detail.jpg "Team Member Detail")