# `base.simline`
contains the simulation lines of the track.

the data section is layed out like this:
|name|type|description
|-|-|-
|count|u32|the amount of lines written
|lines|simline[count]|the list of lines

where each simline is written:
|name|type|description
|-|-|-
|ID|u32|the line's ID
|flags|u8|see [Line Flags](#line-flags)
|x1|f64|the x position of the 1st point
|y1|f64|the y position of the 1st point
|x2|f64|the x position of the 2nd point
|y2|f64|the y position of the 2nd point

## Line Flags
the line flags are a single byte layed out like: `0000DCBA`
|symbol|name|description
|-|-|-
|`A`|red|if `1`, this is an acceleration line.
|`B`|inverted| if `1`, this line is inverted.
|`C`|left extension|if `1`, this line has a left extension.
|`D`|right extension|if `1`, this line has a right extension.
|`0000`|unused|ignored bits

---

*this mod spec is version 0*
