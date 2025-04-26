# `base.startline`
## description
this mod contains the line ID of the "start line". the start offset is set to the first point of this line, minus 25 on the Y axis (thats up 25 units).

if this mod and `base.startoffset` are both present than this mod should take priority when loading, but they generally should be exclusive such that a track is written with at most one of the two.

## data section
name|type|description|
-|-|-|
line ID|`u32`|the ID of the start line|

## meta
```
name = base.startline
version = 0
flags = 00010010 // data | physics
```
