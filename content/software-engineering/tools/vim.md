---
title: "Vim"
date: 2021-02-19T12:00:37-05:00
draft: false
---

## Learn More!
- `vimtutor`
- `:h <string>`- help menu (`:h g`)

## Horizontal Movement
- `hl` - left/right
- `wb` - next/previous word
- `WB` - next/previous whitespace
- `fF` + `<char>` - move to on following/previous charachter in line
- `tT` + `<char>` - move to up to following/previous charachter in line
    - `;` - jump forwards through results
    - `,` - jump backwards through results

## Vertical movement
- `jk` - up/down
- `{}` - move up/down paragraphs (empty lines)
- `ctl+u`/`ctl+d` - page up/down
- `%` - move to next matching {} or ()
- `gg` - jump to beginning of file
- `G` - jump to end of file
- `<int>+G` to go to specified `int` line number 
    - can also use `:` and type line #

## Change Modes
- `ia` - change to insert mode before/after cursor
- `IA` - change to insert mode at the beginning/end of line
- `oO` - change to insert mode below/above current line
- `vV` - select current charachter/line (visual/visual line mode)
- `esc` or `ctl+[` to leave insert mode (return to normal mode)
- `/` or `:` - change to command mode

## Copy/Paste/Delete
- `y` - copy current or following selection
- `yy` - copy current line
- `pP` - paste contents of register below/above current line
- `dD` - delete current or following selection/line
- `dd` - delete current line
- `cC` - delete current or following selection/line and go into insert mode
- `cc` - delete current line and go into insert mode
- `x` - delete current charachter
- `sS` - delete current character/line and go into insert mode
- `di+<char>` - delete all contents between {}, (), "", p (paragraph), etc.
    - also works with `y`, `c`, `a`, and numbers (`d2i{` will delete inner and outer function)

## Undo/Redo
- `u` - undo
- `ctl+r` - redo

## Search/Find
- `*#` - go to next/previous occurance of current selection
- `/` - search for string
- `nN` - move to next/previous result

## Window Operations
- `ctl+w` - followed by:
    - `v` - vertical split
    - `s` - horizontal split
    - `r` - rotate split panes
    - `=` - resize planes to equal sizes
    - `o` - close everything except current buffer
- `:resize <int>` - set number of rows to display
- `:vertical resize <int>` - set number of columns to display
- `:Ex` - open project tree

## Misc.
- `r+<char>` - replace current charachter with following charachter
- `.` - repeat last action
- `ctl+o`/`ctl+p` - jump forwards/backwards in history
- `ctl+^` - hop back and forth between last 2 files opened

## Commands
- `:e src/**/ind + tab` to open a file (better to use scf plugin for `ctl p` fuzzy finder)
- `:set` - set properities (relativenumber, tabstop, backspace, etc.)
- `:highlight` - color settings
- `:syntax enable` - syntax highlighting

## Exit
- `:w` - save (write buffer)
- `:q` - quit
- `;w!` or `:q!` to overwrite permissions

## Useful combos
- `dt}` - delete everything between cursor and closing parenthesis