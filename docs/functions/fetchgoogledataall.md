---
layout: default
title: fetchgoogledataall <span class="new">(Updated)</span>
parent: Functions
nav_order: 3
---

### fetchGoogleDataAll

Use promise to fetch data from Google spreadsheets and return resulting parsed Json array(s).  URL's are formatted to use Google Data Visualization and return one or more JSON data array(s). 

***Usage***

```
fetchGoogleDataAll([url]).then(dataArray => {
	// dataArray[1] has error message
	// dataArray[0][0] has results from 1st URL
	// dataArray[0][1] has results from 2nd URL etc.
	if (dataArrayx[1]) {  // if there was a status error of some kind
		// do something about the error
		return; 
	}
	dataArray = dataArray[0][0].table.rows; // gets the spreadsheet row data

	// Process the data

}
```

**Parameters:**

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>urls</td>
      <td>An array of url's to fetch i.e. ['https:...','https:...']</td>
    </tr>
  </tbody>
</table>

**Preparing url**

```
file_id = '1f3G-ECzjt8p-czZNPyUQGXG8NND016Nue5QypQTf6PQ';
var sheet = 'FAQS';
var url = 'https://docs.google.com/spreadsheets/u/0/d/'
	+ file_id + '/gviz/tq?sheet=' + sheet + '&tqx=out:json&headers=1&tq=' + 
	escape("SELECT A, B, C, D, E WHERE C != 'Yes'");
```

<table class="ws-table-all notranslate"> 
  <tbody>
    <tr class="tableTop">
     <td style="width:120px">Parameter</td>
     <td>Description</td>
    </tr>
    <tr>
      <td>file_id</td>
      <td>Google spreadsheet id</td>
    </tr>
    <tr>
      <td>sheet</td>
      <td>Name of the sheet we are fetching.</td>
    </tr>
    <tr>
      <td>headers</td>
      <td>Set as "1" says that the first row of spreadsheet is a header row.</td>
    </tr>
    <tr>
      <td>tqx</td>
      <td>must be "&tqx=out:json", defines the return value</td>
    </tr>
    <tr>
      <td>tq</td>
      <td>This is an optional SQL like select statement to narrow down returned rows.</td>
    </tr>
  </tbody>
</table>


**Return Value:**

Returns array with two values:
1=Array of data
2=status or error message

**See also**

[Google Query Language Reference](https://developers.google.com/chart/interactive/docs/querylanguage){:target="_blank"}
