# xindex-ko
Korean language module for xindex package

*    written by Dohyun Kim

*    reference: KS X 1026-1:2007

*    usage: `xindex -c ko -l ko file.idx`

*    license: LPPL

This work may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either version 1.3c
of this license or (at your option) any later version.
The latest version of this license is in
  http://www.latex-project.org/lppl.txt
and version 1.3c or later is part of all distributions of LaTeX
version 2006/05/20 or later.

## Tip
If you want symbol-number-english-hangul order of items,
create your own `xindex-ko-SNEH.lua` file containing these lines:
```lua
require "xindex-ko"
SORTendhook = SORTendhook_SNEH
```
and run this command:
```sh
xindex -c ko-SNEH -l ko file.idx
```
.

If you want symbol-number-hangul-english order of items,
create your own `xindex-ko-SNHE.lua` file containing these lines:
```lua
require "xindex-ko"
SORTendhook = SORTendhook_SNHE
```
and run this command:
```sh
xindex -c ko-SNHE -l ko file.idx
```
.

Needless to say, `-l ko` is optional and other xindex options are acceptable.
