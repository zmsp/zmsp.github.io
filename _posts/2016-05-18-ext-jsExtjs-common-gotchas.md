---
title:  "Extjs common gotchas"
excerpt: "Pitfall of Extjs"
header:
    teaser: "/images/extjs.jpg"
    overlay_color: "#3b9943git "
categories: 
  - programming
tags:
  - extjs
  - javascript
---
# tldr: 
- Do not edit Extjs core.
- Do not use ID.
- Keep your code clean and simple.
- Learn and use debugging tools.

# Extjs 

After coding in ExtJs for more then a year, these are my tips. Some of these are from readings others are personal experience. 

### 1. Commas and semicolons are important!
One misplaced or missing comma will result in a blank page. Make sure to use commas after each property except the last property. 

### 2. Naming conventions
Store in the plural. Example: "TeslaCars.js"  
View, in the singular. Example: "TeslaCar.js"   
Model, in the singular. Example: "TeslaCar.js"  
Also lookup variable naming scheme.   

### 3. Global variables
Global variable usage is discouraged.

### 4. Override instead of recreation
Instead of creating a function/view/model/store, try to override existing ones. It will save you a couple lines of code. 


### 5. Alias, Xtypes, Widgets
They could be synonyms of each other depending on usage. Be careful on what you name your components. Make sure not to use any of the reserved xtype/alias.

### 6. Nesting is discouraged
Try to avoid excessive nesting.

### 7. Multiple controllers instead of one monster controller
Try to create multiple controllers if your controller grows for the sake of maintainability

### 8. Folder structures
Look up Extjs recommendation and documents on folder structure before you try to come up with your own scheme.

### 9. Use of ID
Extjs Discourages the use of ID. It causes problems when you create multiple instance of a object. Instead use itemID. 

### 10. Do not edit framework codes
Use override. Or it will be a pain upgrading to a newer version.

### 11. Reuse, reduce recycle
If you find yourself writing same code over the second time, find a way to export the code in a separate xtype so it could be shared across classes. 

### 12. Chrome debugging tools
Learn chrome debugging tools, and familiarize yourself with javascript debugging tools. 


# EXT JS resources
- <http://docs.sencha.com/extjs/4.2.2/#!/example/sandbox/sandbox.html> Live code example. Helpful if you want to play around with code without setting up a dev environment. 
- <https://docs.sencha.com/extjs/4.2.6/> Docs



![extjs logo](/images/extjs.jpg "Some extjs logo")
