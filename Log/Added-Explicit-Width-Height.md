# Added Explicit Width and Height to Images

**Date**: 2025-06-17  
**Issue**:  
PageSpeed Insights flagged: “Image elements do not have explicit width and height.”  
This was causing layout shifts during page load, negatively impacting the CLS score.

**Fix**:  
Manually added `width` and `height` attributes to all major `<img>` tags across site pages.  
Dimensions were set to match actual rendered size to help browsers allocate space.

**Why It Matters**:  
Reduces layout shifts, improving Cumulative Layout Shift (CLS) and overall Core Web Vitals.  
This improves user experience and is considered a search ranking factor.

**Before/After**:  
- CLS score improved from 0.14 → 0.02  
- Layout is now visually stable during page load  
- PageSpeed flag resolved

**Tools Used**:  
- PageSpeed Insights  
- Chrome DevTools  
- Manual HTML editing via VSCode

**Next Steps**:  
- Confirm that future blog images follow the same structure  
- Consider utility class defaults if using a component system or CMS
