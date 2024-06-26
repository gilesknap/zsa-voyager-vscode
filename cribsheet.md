# Combined Keybinding Notes


## Hyper Key bindings for VSCode

Note that hyper 7 and 9 resize ANY pane that you are in. This includes the Explorer and terminals (but vertical only for terminals).

![vscode keybindings](vscode.svg)

-----------------

# Giles Voyager mappings

![right hand keybindings](layout.png)

![left hand keybindings](layoutleft.png)

-----------------

# Keys to remember for vscode

## Breadcrumbs

This deserves its own heading as it is such a useful way to navigate all
the folders in your workspace and all the code sections within each file.

| Key | Action |
| --- | ------ |
| `ctrl shift` `.` | Focus breadcrumbs |
| `↓` `↑` `→` `←`| Navigate breadcrumbs |
| `space` | Open current file or jump to current section |

## Selection management - especially multi cursor

| Key | Action |
| --- | ------ |
| `alt shift` `→` | Expand selection |
| `alt shift` `←` | Shrink selection |
| `alt shift` `i` | add cursors to end of all selected lines (the 2 below can easily do cursors on start)
| `ctrl` `↓` | Add a cursor below |
| `ctrl` `↑` | Add a cursor above |
| `ctrl` `⏎` | Add all found words to selection |
| `ctrl` `D` | Add current word / next matching word to selection |
| `ctrl` `D` | Add current word / next matching word to selection |
| `ctrl` `U` | undo last selection / cursor motion |


e.g. to add '-world' to all instances of 'hello':

- move cursor one of the 'hello',
- `ctrl` `F`
- `alt` `⏎`
- `→` (deselects all 'world' and places the cursors at the right end of each)
- -world

## Navigating the Explorer

And other tree views like search results, git history, etc.

| Key | Action |
| --- | ------ |
| `↓` `↑` `→` `←`| Navigate (shift for multi-select) |
| `letter` | jump to next file starting with  letter |
| `shift letter` | jump to previous file starting with letter |
| `space` | open the current file in a preview editor, keep explorer focus |
| `enter` | open all selected files editors |
| `ctrl` `enter` | open current file in a new editor |
| `alt` `enter` | open current file in a preview editor |
| `F2` | rename current file |
| `Application Key` | Context Menu |

## Navigating code

See [hyperkey.md](hyperkey.md) for navigating changes / errors.

| Key | Action |
| --- | ------ |
| `F12` | Jump to definition |
| `Application Key` | Menu for ALL code inspection options |

## Terminals

| Key | Action |
| --- | ------ |
| `ctrl shift`  `` ` `` | Open new terminal (back tick) |
| `ctrl page` `up`/`down` | Switch to prev / next Terminal Group |
| `ctrl` `↑` / `↓` | Scroll to previous / next command input |
| `ctrl shift` `↑` / `↓` | Move SELECTION to previous / next command output |
| `ctrl shift` `C` / `V` | Copy / Past SELECTION |

To get a terminal command output into an editor window:

- Select the one you want with ctrl arrows and ctrl shift arrows.
- `ctrl shift` `C` to copy
- `ctrl` `1` switch to fist editor group
- `ctrl` `N` for new window
- `ctrl` `V` to paste

Above is a good candidate for a keyboard macro if you have such a capability.

## Menus

| Key | Action |
| --- | ------ |
| `alt` | Show menu bar |
| `alt shift` `O` | Open Remotes / Dev Containers menu |

## Side Bars

| Key | Action |
| --- | ------ |
| `ctrl B` | show/hide primary side bar (usually left) |
| `ctrl alt B` | show/hide secondary side bar (usually right) |
