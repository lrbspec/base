# `base.startline`
## description
this mod contains the line ID of the "start line". the start offset is set to the first point of this line, minus 25 on the Y axis (which means upwards 25 units).

if this mod and `base.startoffset` are both present, then this mod should take priority when loading, but they generally should be exclusive such that a track is written with at most one of the two.

## data layout
name|type|description|
-|-|-|
line ID|`u32`|the ID of the start line|

## meta
```
name = base.startline
version = 0
flags = 00010010 // data | physics
dependencies = base.simline version 1 or base.scnline version 1 (the line ID may refer to a scenery or simulation line. it isnt technically required for both mods to be present but if they are then order this one after both of them to be safe)
```
