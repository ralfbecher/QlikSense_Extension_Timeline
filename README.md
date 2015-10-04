Qlik Sense Extension Timeline
=============================

This extension implements vis.js timeline http://visjs.org/docs/timeline/. It is an interactive chart to visualize data items in time. The items can take place on a single date, or have a start and end date (a range).  You can freely move and zoom in/out the timeline by dragging and scrolling. 

![QlikSense Extension Timeline](Timeline.gif)

![QlikSense Extension Timeline](Screenshot2.PNG)

Dimensions:
----------------------
1. Dimension: Reference ID, numeric (Event ID or else) or String
2. Dimension: Item Content, text
3. Dimension: Start Date
4. Dimension: End Date (optional, null if omitted)
5. Dimension: Item Type (box (default), point, range, background)

Measures:
----------------------
1. Measure: title text for hover popup (optional), default title is start date
2. Measure: CSS class name for styling or number 1 to 10 for CSS class color-a to color-j which are configured for Qlik Sense diverging colors (blue-to-red, optional)
3. Measure: group name to group items in "swim lanes" (optional)

Additional Properties:
----------------------
1. Axis Orientation : top, bottom (default), both, none
2. Item orientation : top, bottom (default)
3. Group Sorting    : Ascending, Descending
4. Localization     : choose local for localized date and timestamp formatting (default: en-gb)
5. Reverse Color    : reverse Qlik Sense diverging color (red-to-blue)
6. Apply CSS for Background : apply CSS class to background items (default: true)