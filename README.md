# vim

> [cheatsheet](https://vim.rtorr.com/)

## Modes

- `v` - visual mode
- `:` - command mode
- `i` - insert mode
- `esc` - back to normal mode

## Normal Mode

#### Basic Navigation

- `h` → left (going home)
- `j` → down (jumping down)
- `k` → up (kicking up)
- `l` → right
- `5k` → 5 lines up

#### Navigate by word

- `b` → Move backword by word (letters,numbers and underscores)
- `B` → Move backword by WORD (till whitespace)
- `w` → Move forward by word
- `W` → Move forward by WORD

#### Move to specific position

- `$` → Move to the end of the line
- `^` → Move to the first non-blank character of the line
- `0` → Move to the start of the line

- `ctrl+u` → page up
- `ctrl+d` → page down

- `5G` → move to 5th line

- `H` → Move to the Top of the screen (High)
- `M` → Move to the Middle of the screen (Middle)
- `L` → Move to the Low of the screen (Low)

#### Delete & Correct

- `x` → delete a character
- `r` → replace a character
- `D` or `d$` → delete rest of the line
- `C` or `c$` → delete rest of the line and insert mode
- `dd` → delete the current line
- `5dd` → delete the next 5 line
- `cw` → correct the token (delete + insert)
- `cW` → correct the word
- `cc` → correct the line

#### Copy, Paste, Undo & Redo

- `u` → undo
- `ctrl + r` → redo

- `yy` → copy line (y for yank)
- `yw` → copy token
- `yW` → copy word
- `p` → paste the last thing that was deleted or copied

## Insert Mode

- `i` → insert before the cursor
- `I` → insert at the beginning of the line
- `a` → insert (append) after the cursor
- `A` → insert (append) at the end of the line
- `o` → append (open) a new line below the current line
- `O` → append (open) a new line above the current line
- `Ctrl + h` - delete the character before the cursor during insert mode
- `Ctrl + w` - delete word before the cursor during insert mode
- `Ctrl + t` - indent (move right) line one shiftwidth during insert mode
- `Ctrl + d` - de-indent (move left) line one shiftwidth during insert mode

## Commands

- `:w` - write (save) the file, but don't exit
- `:w !sudo tee %` - write out the current file using sudo
- `:wq` or `:x` or `ZZ` - write (save) and quit
- `:q` - quit (fails if there are unsaved changes)
- `:q!` or `ZQ` - quit and throw away unsaved changes
- `!node filename.ext` - run a file
- `:wqa` - write (save) and quit on all tabs
