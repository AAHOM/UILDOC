---
layout: default
title: Carousel  <span class="new">(Updated)</span>
parent: Components
nav_order: 7
---

### Carousel

The ***createCarousel*** requires that at least one summary carousel is defined in the same SquareSpace page section.   

***Cook book to create a carousel summary block***
- Edit the page
- Click the "+" sign where you want the carousel to appear
- Select **Summary Block**
- Under ***content*** 
	- select the appropriate blog to display
	- Primary Metadata: None
	- Secondary Metadata: None
	- Filter Items: If needed
- Under ***Design*** 
	- Select Carousel
	- Number of items: 30 (max)
	- Items per Row: 3 
	- Aspect Ratio: 3:2 Standard
	- Text: L (Left align)
	- Header Text: Featured (or whatever you want)
	- Title: On
	- Featured Image: On
	- Excerpt: On
	- Read More Link: On
	- Set Read More Link Text: Read More
	- Metadata Position: Below Content
	- Size and Spacing: Column Width=280px, gutter width=60px, Use Columns Number=Off
- Under ***Lazy Settings***
	- Ignore for now, leave off
- Under ***Additional***
	- Ignore for now, leave off

Once the carousel summary block has been defined, insert a code block to 
transform the carousel to a Slick plugin carousel.  

***Cook book to add Slick Carousel***
- Edit the page
- Click a "+" sign just above the carousel summary block, in the same section 
- Select "Code"
- Paste the following code block
- Adust parameters as needed

**Code block for slick carousel**
```
<script>
$(document).ready(function(){
    createCarousel ('#announcementCarousel');    
});
</script>
<div id="announcementCarousel"></div>
``` 

**Overrides:**

None

**Usage:**

*createCarousel(SelectorID, ContainerNumber)*

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
    <tr>
      <td><em>ContainerNumber</em></td>
      <td>Optional, zero or greater number.  Needed if more than one carousel exists in the same page section.  Zero (default) referes to the first carousel in the section, and so on.
      </td>
    </tr>
  </tbody>
</table>

**Return Value:**

None


**Additional Carousel Dependancies**

- Slick plugin

**Example Screenshot**

![Alt Slick Carousel](../../assets/images/slick_carousel.jpg "Slick Carousel")
