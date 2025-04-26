# `base.startoffset`
## description
this mod contains the x and y coordinates of the start offset of the track. 

if `base.startline` is present then that mod takes priority and overwrites this value, but writing implementations should write at most one of the two.

the omission of both this mod and `base.startline` implies a start offset of (0, 0) by default

## data section
name|type|description|
-|-|-|
X|`f64`|the X coordinate of the start offset|
Y|`f64`|the Y coordinate of the start offset (remember +Y is down)|

## meta
```
name = base.startoffset
version = 0
flags = 00010010
```
