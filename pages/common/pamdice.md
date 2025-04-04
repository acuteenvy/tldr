# pamdice

> Slice a Netpbm image vertically or horizontally.
> See also: `pamundice`.
> More information: <https://netpbm.sourceforge.net/doc/pamdice.html>.

- Slice a Netpbm image such that the resulting tiles have the specified height and width:

`pamdice {{[-o|-outstem]}} {{path/to/filename_stem}} {{[-he|-height]}} {{value}} {{[-w|-width]}} {{value}} {{path/to/input.ppm}}`

- Make the produced pieces overlap by the specified amount horizontally and vertically:

`pamdice {{[-o|-outstem]}} {{path/to/filename_stem}} {{[-he|-height]}} {{value}} {{[-w|-width]}} {{value}} {{[-ho|-hoverlap]}} {{value}} {{[-vo|-voverlap]}} {{value}} {{path/to/input.ppm}}`
