# Random Identifier Generator

Vim plugin that inserts random identifiers for your codes on insert mode.

I could say this is one of the best plugin to make code unmaintainable.

## Installation

copy `plugin/rig.vim` to `~/.vim/plugin`

## Usage

- Ctrl+z,z

    Insert an identifier with default pattern.

- Ctrl+z,x

    Insert an identifier with a fixed size (default is 3).

- Ctrl+z,c

    Clear identifier histroy.

- Ctrl+z,i

    Insert an identifier with certain length (1~9).

## Configuration

You can configure fixed size used by ctrl+z,x.
Or generation patterns.

```vim
  let g:rig_fixed_size = 3
```

The default generation setting will generate
an identifier with a length of 1 to 3.

```vim
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
