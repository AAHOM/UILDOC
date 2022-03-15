---
layout: default
title: jsdelivr
parent: Services
nav_order: 6
---

### jsdelivr

**jsdelivr** is a CDN service that we are using to serve the custom javascript and styles for the website. jsdelivr works directly with GitHub, with no configuration or accounts needed. 

As an example, the following links can be found in the header ocde injection block of the SquareSpace site:

```
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/AAHOM/UIL@2e7344a/unity.min.js"></script>
<link rel='stylesheet' href="https://cdn.jsdelivr.net/gh/AAHOM/UIL@3b7af82/styles.min.css" />
```

In the above example:

- **AAHOM/UIL** - is the GitHub account and repository that hold the javascript and css style files.
- **@2e7344a** and **@3b7af82** refer to the commit key for the respective files.  
- **unity.min.js** and **styles.min.css** are the files to be linked. 

***Note:*** The commit key is an important part.  Each time a change is made to a file in the GitHub repository a new key for that file is generated.  For jsdelivr to fetch the latest changes, that key needs to be updated in the SquareSpace Code Injection header block.  