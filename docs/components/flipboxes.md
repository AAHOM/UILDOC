---
layout: default
title: Flip Boxes <span class="new">(Updated)</span>
parent: Components
nav_order: 9
---

### Flip Boxes

Home page flip boxes for Visit, Learn and Support.

***Cook book***
- Edit the page
- Click a "+" sign where you want to insert 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for flip cards**
```
<script>
$( document ).ready(function() {
  build_flipcards("#flexbox"); 
});
</script>
<div id=flexbox></div>
```

**Overrides:**

None

**Usage:**

*build_flipcards(Selector, Boxnumber)*

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
    <tr class="w3-white">
      <td>Boxnumber</td>
      <td>Box number from column A in spreadsheet.  Default=1.  The spreadsheet can contain multiple variations of the flipboxes, each with unique number. 
      </td>
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
      <td>Flip Boxes</td>
    </tr>
    <tr>
      <td>Folder</td>
      <td><a href="https://drive.google.com/drive/folders/1YaVLSr9quHsbMDChBrlZUjpI_ZeG0cG-" target="_blank">UIL_Web_Site_Docs</a></td>
    </tr>
    <tr>
    	<td>Link</td>
    	<td><a href="https://docs.google.com/spreadsheets/d/1wEfSb4Dnjz-eNEayaNiiws3ta1ZEueiQyG5-BTWSXag/edit#gid=851926596" target="_blank">Flip Boxes Spreadsheet</a></td>
    </tr>
    <tr>
      <td>ID</td>
      <td>1wEfSb4Dnjz-eNEayaNiiws3ta1ZEueiQyG5-BTWSXag</td>
    </tr>
    <tr>
      <td>Sheet Name</td>
      <td>Cards2</td>
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
		<td>Box</td>
		<td>Box number from column A in spreadsheet.  Default=1.  The spreadsheet can contain multiple variations of the flipboxes, each with unique number.
		</td>
	</tr>
	<tr>
		<td>B</td>
		<td>Card</td>
		<td>This is the order that the cards are presented. Expecting a number.</td>
	</tr>
	<tr>
		<td>C</td>
		<td>Caption</td>
		<td>Text highlighted on front of card.</td>
	</tr>
	<tr>
		<td>D</td>
		<td>Label</td>
		<td>Not used</td>
	</tr>
	<tr>
		<td>E</td>
		<td>link</td>
		<td>Page link</td>
    </tr>
    <tr>
		<td>F</td>
		<td>Background color</td>
		<td>rgb color code, ie. rgb(102, 102, 102)</td>
    </tr>
    <tr>
		<td>G</td>
		<td>Color</td>
		<td>Color of text message</td>
	</tr>
    <tr>
		<td>H</td>
		<td>Message</td>
		<td>Text message on flip side</td>
    </tr>
    <tr>
		<td>I</td>
		<td>Image1</td>
		<td>Link to image 1</td>
    </tr>
    <tr>
		<td>J</td>
		<td>Image2</td>
		<td>Link to image 2</td>
    </tr>
    <tr>
		<td>K</td>
		<td>Image3</td>
		<td>Link to image 3</td>
    </tr>
    <tr>
		<td>L</td>
		<td>Image4</td>
		<td>Link to image 4</td>
    </tr>
    <tr>
		<td>M</td>
		<td>Image5</td>
		<td>Link to image 5</td>
    </tr>
    <tr>
		<td>N</td>
		<td>Image6</td>
		<td>Link to image 6</td>
    </tr>
    <tr>
		<td>O</td>
		<td>Image7</td>
		<td>Link to image 7</td>
    </tr>
    <tr>
		<td>P</td>
		<td>Image8</td>
		<td>Link to image 8</td>
    </tr>
  </tbody>
</table>

**Example Screenshot**

![Alt Home Page Flip Boxes](../../assets/images/flip_boxes.jpg "Home Page Flip Boxes")