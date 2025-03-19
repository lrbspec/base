# `base.startoffset`
this mod contains two f64's for the x and y coordinate of the start offset of the track. 
if `base.startline` is present then that mod takes priority and overwrites this value, but writing implementations should only write one of the two.

the data section is layed out like this:
name|type|description|
-|-|-|
X|`f64`|the X coordinate of the start offset|
Y|`f64`|the Y coordinate of the start offset (remember +Y is down)|
***
*this spec is version 0*
