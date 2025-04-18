# bmaptool

> Create or copy block maps intelligently (designed to be faster than `cp` or `dd`).
> More information: <https://manned.org/bmaptool>.

- Output a blockmap file from image file:

`bmaptool create {{[-o|--output]}} {{blockmap.bmap}} {{source.img}}`

- Copy an image file into sdb:

`bmaptool copy --bmap {{blockmap.bmap}} {{source.img}} {{/dev/sdb}}`

- Copy a compressed image file into sdb:

`bmaptool copy --bmap {{blockmap.bmap}} {{source.img.gz}} {{/dev/sdb}}`

- Copy an image file into sdb without using a blockmap:

`bmaptool copy --nobmap {{source.img}} {{/dev/sdb}}`
