# Viewport Meta Tag Implemented Across Site

**Date**: 2025-06-17  
**Issue**:  
PageSpeed Insights flagged: “No `<meta name='viewport'>` tag found.”  
Without this tag, pages rendered incorrectly on mobile devices, causing layout issues and poor usability — especially in Google's mobile-first indexing context.

**Fix**:  
Added the following tag to the `<head>` section of all static HTML pages:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
