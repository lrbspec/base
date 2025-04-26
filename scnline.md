# `base.scnline`
## description
contains the scenery lines of the track.

## data section
|name|type|description
|-|-|-
|count|u32|the amount of lines written
|lines|scnline[count]|the list of lines

where each scnline is written:
|name|type|description
|-|-|-
|ID|u32|the line's ID
|x1|f64|the x position of the 1st point
|y1|f64|the y position of the 1st point
|x2|f64|the x position of the 2nd point
|y2|f64|the y position of the 2nd point

## meta
```
name = base.scnline
version = 0
flags = 00011000 // data | scenery
```
