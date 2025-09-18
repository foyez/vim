# vim

> [cheatsheet](https://vim.rtorr.com/)

---

## 🔀 Modes

* `v` → **Visual mode** (select text)
* `i` → **Insert mode**
* `:` → **Command mode**
* `Esc` → back to **Normal mode**

---

## 🚀 Normal Mode

### Navigation

* **Characters & Lines**

  * `h` ← left (home)
  * `l` → right
  * `j` ↓ down
  * `k` ↑ up
  * `5j` / `5k` → move 5 lines down/up

* **Words & WORDS**

  * **word** = till letters, numbers, and unserscores
  * **WORD** = till whitespace
  * `w` / `W` → beginning of next word / WORD
  * `e` / `E` → end of current/next word / WORD
  * `b` / `B` → beginning of current/previous word / WORD

* **Lines**

  * `0` → start of line
  * `^` → first non-blank char
  * `$` → end of line

* **Screens**

  * `Ctrl-u` → half-page up
  * `Ctrl-d` → half-page down
  * `Ctrl-b` → page back
  * `Ctrl-f` → page forward
  * `H` / `M` / `L` → top / middle / bottom of screen

* **Paragraphs & File**

  * `{` / `}` → prev/next paragraph
  * `gg` / `G` → top / bottom of file
  * `:{n}` / `{n}G` → go to line n

---

### Jump List & Navigation

* `Ctrl-o` → jump **backward** (older position)
* `Ctrl-i` → jump **forward** (newer position)
* `''` → jump to line of last cursor position
* ` `` ` → jump to exact last cursor position

👉 **Pro tip:** Think of `Ctrl-o`/`Ctrl-i` as **Back/Forward buttons** in a browser.

---

### Lookups & Tags

* `K` → open keyword documentation (e.g. man page or `:help`)
* `gd` → go to local declaration
* `gD` → go to global declaration
* `Ctrl-]` → jump to tag under cursor
* `Ctrl-t` → jump back from tag

---

### Copy / Paste / Delete / Change

* `yy` / `Y` → yank line
* `yw` / `yW` → yank word / WORD
* `p` / `P` → paste after / before
* `dd` / `5dd` → delete line(s)
* `cw` / `cW` → change word / WORD
* `cc` → change line

👉 **Pro tip:** `y3w` → yank 3 words, `d5W` → delete 5 WORDs, `c2e` → change until end of second word, `v4e` → visually select up to the end of the fourth word

---

### Indentation

* `>>` / `<<` → indent / de-indent line
* `>` / `<` in Visual mode → indent selection
* `=` → auto-indent selection (use `gg=G` for entire file)

---

### Undo & Redo

* `u` → undo
* `Ctrl-r` → redo

---

### Repeat

* `.` → repeat last command
* `@:` → repeat last command-line command

---

### Marks

* `ma` → mark cursor as `a`
* `'a` → jump to mark `a` (line)
* `` `a `` → jump to mark `a` (exact column)
* ` `` ` → jump back to last position

---

### Buffers & Windows

* `:ls` → list buffers
* `:b{n}` → go to buffer {n}
* `:bd` → close buffer
* `:new` / `:vnew` → split
* `Ctrl-w h/j/k/l` → move between splits
* `gt` / `gT` → next / prev tab

---

### Search & Replace

* `/pattern` → search forward

* `n` / `N` → next/prev match

* `*` → search word under cursor forward

* `#` → search word under cursor backward

* `:%s/old/new/g` → replace all

* `:6,10s/old/new/g` → replace in lines 6–10

---

## ✍️ Insert Mode

* `i` / `I` → insert before cursor / at start of line
* `a` / `A` → append after cursor / at end of line
* `o` / `O` → new line below / above
* `Ctrl-h` → delete previous char
* `Ctrl-w` → delete previous word
* `Ctrl-u` → delete to line start
* `Ctrl-t` / `Ctrl-d` → indent / de-indent line

---

## ⚙️ Commands

* `:w` → save
* `:q` → quit
* `:wq` / `:x` / `ZZ` → save + quit
* `:q!` / `ZQ` → quit without saving
* `:wqa` → save + quit all

---

## ⚡ Power Moves

* `%` → jump to matching bracket
* `g;` / `g,` → jump to older/newer change
* `Ctrl-g` → show file + cursor position info
* `:noh` → clear search highlights

---
