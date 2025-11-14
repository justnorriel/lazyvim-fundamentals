# LazyVim Basic Keyboard Shortcuts

> **Note:** `Space` is your main leader key in LazyVim

## General Navigation

### Basic Movement
- `h` - Move left
- `j` - Move down
- `k` - Move up
- `l` - Move right
- `w` - Jump to start of next word
- `b` - Jump to start of previous word
- `e` - Jump to end of word
- `0` (zero) - Jump to start of line
- `Shift + 4` ($) - Jump to end of line
- `g g` (press g twice) - Go to first line
- `Shift + g` (G) - Go to last line
- `{number} Shift + g` - Go to line number (e.g., `50` then `Shift + g`)
- `Ctrl + d` - Scroll down half page
- `Ctrl + u` - Scroll up half page
- `Ctrl + f` - Scroll down full page
- `Ctrl + b` - Scroll up full page

## Modes

- `i` - Insert mode (before cursor)
- `a` - Insert mode (after cursor)
- `Shift + i` (I) - Insert at beginning of line
- `Shift + a` (A) - Insert at end of line
- `o` - Open new line below
- `Shift + o` (O) - Open new line above
- `v` - Visual mode (character selection)
- `Shift + v` (V) - Visual mode (line selection)
- `Ctrl + v` - Visual block mode (column selection)
- `Esc` or `Ctrl + [` - Return to normal mode

## File Operations

- `Space f f` - Find files (Fuzzy finder)
- `Space f r` - Recent files
- `Space f g` - Live grep (search text in all files)
- `Space f b` - Find buffers (open files)
- `Space f n` - New file
- `:w` then `Enter` - Save file (write)
- `:q` then `Enter` - Quit
- `:wq` or `:x` then `Enter` - Save and quit
- `:q!` then `Enter` - Quit without saving (force quit)

## Window Management

- `Space w w` - Switch between windows
- `Space w d` - Delete/close window
- `Space w -` - Split window horizontally (below)
- `Space w |` - Split window vertically (right)
- `Ctrl + h` - Move to left window
- `Ctrl + j` - Move to bottom window
- `Ctrl + k` - Move to top window
- `Ctrl + l` - Move to right window

## Buffer Management

- `Space b b` - Switch buffers (open files list)
- `Space b d` - Delete/close buffer
- `[ b` - Previous buffer (open bracket + b)
- `] b` - Next buffer (close bracket + b)

## File Explorer (Neo-tree)

- `Space e` - Toggle file explorer
- `Space f e` - Toggle file explorer (focused on current file)

## Editing

### Basic Editing
- `x` - Delete character under cursor
- `d d` (press d twice) - Delete entire line
- `Shift + d` (D) - Delete from cursor to end of line
- `y y` (press y twice) - Yank/copy entire line
- `Shift + y` (Y) - Yank/copy to end of line
- `p` - Paste after cursor
- `Shift + p` (P) - Paste before cursor
- `u` - Undo
- `Ctrl + r` - Redo
- `.` (period) - Repeat last command

### Text Objects (combine with c=change, d=delete, y=yank/copy, v=visual)
- `c i w` - Change inside word
- `d i w` - Delete inside word
- `y i w` - Yank/copy inside word
- `c i "` - Change text inside quotes
- `d i (` - Delete text inside parentheses
- `v i {` - Visual select inside braces

## Search and Replace

- `/pattern` then `Enter` - Search forward
- `?pattern` then `Enter` - Search backward
- `n` - Next search result
- `Shift + n` (N) - Previous search result
- `Shift + 8` (*) - Search word under cursor forward
- `Shift + 3` (#) - Search word under cursor backward
- `Space s h` - Clear search highlight
- `:%s/old/new/g` then `Enter` - Replace all occurrences in file
- `:%s/old/new/gc` then `Enter` - Replace all with confirmation for each

## Code Actions

- `Space c a` - Code actions (fix, refactor suggestions)
- `Space c r` - Rename symbol/variable
- `g d` - Go to definition
- `g r` - Go to references (where else this is used)
- `Shift + k` (K) - Hover documentation (info popup)
- `[ d` - Previous diagnostic/error
- `] d` - Next diagnostic/error
- `Space c d` - Show line diagnostics/errors

## Terminal

- `Space f t` - Open terminal (at root directory)
- `Space f Shift + t` - Open terminal (at current directory)
- `Ctrl + /` - Toggle terminal

## Git

- `Space g g` - Open LazyGit (full git interface)
- `Space g b` - Git blame line (see who wrote this)
- `] h` - Next git hunk/change
- `[ h` - Previous git hunk/change
- `Space g p` - Preview git hunk/change
- `Space g r` - Reset git hunk/change

## LSP (Language Server Protocol - Code Intelligence)

- `g Shift + d` (gD) - Go to declaration
- `g d` - Go to definition
- `g i` - Go to implementation
- `g y` - Go to type definition
- `g r` - Show all references
- `Shift + k` (K) - Hover documentation
- `Space c f` - Format code (auto-format)
- `Space c a` - Code actions (suggestions)

## Miscellaneous

- `Space l` - Lazy (plugin manager interface)
- `Space q q` - Quit all windows
- `Space u i` - Inspect position (syntax info)
- `Space u Shift + i` - Inspect tree (syntax tree)
- `Space Shift + l` (L) - LazyVim changelog
- `Space Tab` - Switch to last tab
- `Space |` - Split window vertically (right)
- `Space -` - Split window horizontally (below)

## Quick Tips

- **Space** is your leader key - press it and wait a moment to see available shortcuts
- Press `Space ?` to see all available keymaps
- Most commands can be preceded by a number for repetition:
  - `3 d d` - Delete 3 lines
  - `5 j` - Move down 5 lines
  - `2 w` - Jump forward 2 words
- **Escape** gets you back to normal mode from any mode
- When in doubt, press `Esc` to return to safety!

## Common Workflows

### Opening and Editing Files
1. `Space f f` - Find and open a file
2. `i` - Start editing (insert mode)
3. Make your changes
4. `Esc` - Back to normal mode
5. `:w` `Enter` - Save
6. `:q` `Enter` - Quit

### Searching and Replacing
1. `/searchterm` `Enter` - Search
2. `n` - Jump to next occurrence
3. `:%s/old/new/gc` `Enter` - Replace with confirmation
4. `y` or `n` for each occurrence

### Working with Multiple Files
1. `Space f f` - Open first file
2. `Space f f` - Open another file
3. `Space b b` - Switch between open files
4. `Ctrl + h/j/k/l` - Navigate between split windows