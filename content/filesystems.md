---
layout: default
title: Working with files and filesystems
nav_order: 8
---
# Working with files and filesystems

Basic file redirection:

- `>`: Redirect to a file
- `<`: Take input from a file
- `|`: Send output to another program
- `>>`: **append** to an existing file
- use `tee` to display output but **also** write it to a file:
  - example: `ls | tee outfile.txt`

Examples:

```bash
date > test.md # Create a file called "test.md" with the current date
date >> test.md # Append the date to an existing file "test.md"
date | grep Fri # Look for a string "Fri" in the output of date
sort < test.md # Sort the contents of test.md
```

Other ways of working with files:

- `du` and `df`: show directory and disk usage
- `tree`: list directory contents in a tree-like format
- `mc`: (Midnight Commander) visual shell

Apart from typing commands to view the structure and contents of the filesystem, it is also possible to visually interact with directories of files using tools like [Midnight Commander](https://midnight-commander.org/).

Midnight Commander can be accessed using the `mc` command, which opens up a split view of the current directory. Both panes of this view can be configured to view different locations in your filesystem, or to perform other operations like viewing files.

Midnight Commander basics:

- `F9`: Access menu
- `Alt+.`: Hide hidden files and directories
- `F5`: Copy files from one pane to the other
- `F6`: Rename/move files
- `F7`: Make new directory
- `+` and `-` to select files, `*` to invert selection
- `Alt+C`: Quick change directory
