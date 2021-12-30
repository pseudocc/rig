# Random Identifier Generator

Insert a random identifier for your code on insert mode.

## Installation

copy `plugin/rig.vim` to `~/.vim/plugin`

## Usage

- Ctrl+i

    Insert an identifier

- Ctrl+Shift+i

    Clear history and insert an identifier

## Configuration

The default generation setting will generate
an identifier with a length of 1 to 3.

```vimscript
" Pattern for generation
" u - upper case
" l - lower case
" d - digit
" x - blank
let g:rig_patterns = ['l', 'lldux', 'lddx']
let g:rig_patconf = {
  \'l': [97, 26],
  \'u': [65, 26],
  \'d': [48, 10],
  \'x': [0, 1]
  \}
```
