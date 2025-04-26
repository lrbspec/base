# `base.gridver`
## description
indicates the grid algorithm version of the track, out of the three values that existed in the flash version.

## data section
the data section is layed out like this:
name|type|description|
-|-|-|
grid version|`u8`|the grid algorithm version used by the track, see below for values|

the possible values are:
name|value|
-|-|
6.2|`0`|
6.1|`1`|
6.0|`2`|

all other values are undefined and should be rejected when loading.


## meta
```
name = base.gridver
version = 0
flags = 00010010 // data | physics
```
