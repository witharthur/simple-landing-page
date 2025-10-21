1. What is Semantic HTML?
Semantic HTML uses HTML elements that clearly describe their meaning and purpose to both the browser and developer. Instead of using generic <div> or <span> tags everywhere, semantic HTML uses meaningful tags like <header>, <nav>, <article>, <section>, <footer>, etc.
Benefits:

Improves accessibility for screen readers
Better SEO (search engines understand content structure)
More readable and maintainable code
Helps developers understand the structure quickly


2. How does CSS Flexbox differ from Grid?
Both Flexbox and Grid are layout systems, but they serve different purposes:
Flexbox (1-Dimensional Layout)

Designed for layouts in one direction (row or column)
Best for aligning items in a single axis
Great for navigation bars, button groups, card layouts
Content-first approach (items control the layout)
Items can grow, shrink, and wrap dynamically

Grid (2-Dimensional Layout)

Designed for layouts in both directions (rows and columns simultaneously)
Best for complex page layouts
Great for entire page structures, dashboards, magazine-style layouts
Layout-first approach (you define the grid structure)
Provides precise control over rows and columns


3. What are Media Queries?
Media queries are CSS techniques that allow you to apply different styles based on device characteristics like screen width, height, orientation, or resolution. They are essential for creating responsive designs that adapt to different devices and screen sizes. Media queries use the @media rule to conditionally apply CSS styles when certain conditions are met, such as minimum or maximum viewport width, device orientation, or pixel density.

4. How do you make a website responsive?
Making a website responsive involves several techniques to ensure it works well on all device sizes:
Key Techniques:

Mobile-First Approach: Start designing for mobile devices, then scale up for larger screens
Flexible Layouts: Use relative units like percentages, em, rem, vw, vh instead of fixed pixels
Media Queries: Apply different styles for different screen sizes and breakpoints
Responsive Images: Use max-width: 100% and the srcset attribute for different resolutions
Flexible Grid Systems: Utilize Flexbox or CSS Grid for adaptable layouts
Viewport Meta Tag: Include the viewport meta tag in HTML for proper mobile rendering
Fluid Typography: Use relative font sizes that scale with viewport size
Breakpoints: Define strategic breakpoints for tablets, desktops, and large screens


5. Explain the Box Model
The CSS box model describes how every HTML element is represented as a rectangular box. Each box consists of four parts from inside out:
Four Components:

Content: The actual content area containing text, images, or other elements
Padding: Transparent space between content and border, inside the element
Border: A line surrounding the padding, can have color, width, and style
Margin: Transparent space outside the border, separating the element from others

Box-Sizing Property:

content-box (default): Width and height only apply to content area
border-box: Width and height include padding and border

The total element width equals content width plus left and right padding, borders, and margins. Understanding the box model is crucial for precise layout control and avoiding unexpected spacing issues.

6. What is the difference between Classes and IDs in CSS?
Classes (.classname)

Can be reused on multiple elements throughout the page
Multiple classes can be applied to a single element
Less specific in CSS specificity hierarchy
Used for styling groups of similar elements
Best practice for most styling needs

IDs (#idname)

Should be unique, appearing only once per page
Only one ID can be applied per element
More specific in CSS specificity hierarchy
Used for unique elements and JavaScript targeting
Often used for page anchors and fragment identifiers


Best Practice: Use classes for styling and IDs sparingly for unique page elements or JavaScript hooks.


7. How can you optimize CSS for performance?
File Size Optimization:

Remove unused CSS rules and dead code
Minify CSS files for production
Use shorthand properties to reduce code length
Eliminate duplicate rules and consolidate styles

Code Efficiency:

Avoid deep nesting and overly complex selectors
Simplify selector specificity
Avoid universal selectors that target all elements
Use efficient descendant selectors

Loading Optimization:

Inline critical CSS for above-the-fold content
Defer non-critical CSS loading
Use CSS sprites for combining multiple images
Implement code splitting for large applications

Performance Best Practices:

Minimize expensive properties like multiple shadows and filters
Avoid layout-triggering properties in animations
Use GPU-accelerated properties like transform and opacity
Leverage CSS variables for reusability
Prefer modern layout methods like Grid and Flexbox over floats


8. What is the difference between Relative and Absolute positioning?
Relative Positioning (position: relative)

Element is positioned relative to its normal position in the document flow
The element still occupies its original space
Other elements are not affected and don't fill the space
Can be offset using top, right, bottom, left properties
Often used to create a positioning context for child elements

Absolute Positioning (position: absolute)

Element is positioned relative to its nearest positioned ancestor
If no positioned ancestor exists, it positions relative to the document body
Element is completely removed from the normal document flow
Other elements behave as if the absolutely positioned element doesn't exist
The space it would have occupied is filled by surrounding elements
Can be positioned precisely using top, right, bottom, left properties


Key Difference: Relative positioning maintains document flow space, while absolute positioning removes the element from flow entirely.


9. How does the z-index property work?
The z-index property controls the stacking order of positioned elements along the z-axis (depth). Elements with higher z-index values appear in front of elements with lower values.
Key Characteristics:

Only works on positioned elements (relative, absolute, fixed, sticky)
Does not work on static positioning (the default)
Default value is auto, which is equivalent to 0
Can accept positive, negative, or zero values
Creates new stacking contexts in certain situations

Stacking Contexts:
Certain CSS properties create new stacking contexts that affect how z-index works. Elements inside a stacking context are contained within that context, meaning a child element's z-index only compares to siblings within the same stacking context, not to elements outside it.

Important: A high z-index value on a child element won't make it appear above elements outside its parent's stacking context if the parent has a lower z-index.


10. What is the difference between Padding and Margin?
Padding

Space inside the element between content and border
Part of the element's clickable and hoverable area
Affected by the element's background color and images
The background extends through the padding area
Generally cannot have negative values
Included in the element's total size calculation

Margin

Space outside the element between border and other elements
Not part of the element's clickable or hoverable area
Always transparent, showing the parent's background
Creates separation between adjacent elements
Can have negative values for overlapping effects
Subject to margin collapse in vertical layouts
