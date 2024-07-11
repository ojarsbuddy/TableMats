# Table Mats

Resolved the issue with Evince Document Viewer. Turns out the application uses the various bounding boxes in the postscript file to make the visible window.

from

```%%BoundingBox: 0 0 400 796```

```%%PageBoundingBox: 0 0 400 796```  

to

```%%BoundingBox: 0 0 612 792```

```%%PageBoundingBox: 0 0 612 792```  

For 72 parts per inch in postscript, that gets us 792 parts in 11 inches and 612 parts in 8.5 inches.
