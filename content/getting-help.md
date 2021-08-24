---
layout: default
title: Getting help
nav_order: 6
---
# Getting help on the command-line

You may already be familiar with some basic ways to get help in the shell, e.g.:

* `help`: Show list of shell commands
* `whatis`: Display one-line manual page descriptions
* `apropos`: Search the command manual page names and descriptions
* `man`: View system reference manuals for individual commands
  * `man ls`: View manual for `ls` command
  * `man hier`: Description of the *nix filesystem hierarchy

When encountering a new command, it is a good habit to quickly check what it does using `whatis` or `man` before using it. This can help avoid any unintended side effects that can occur when copy-pasting commands to the terminal (which is not recommended).

## Interactive system documentation

Apart from the above, there are also other ways to get help while using the command-line.

First, there is a comprehensive and interactive guide to the Unix Shell and GNU CoreUtils that is accessible by simply typing `info`.

Within `info`, you can move around with the arrow keys on your keyboard and select underlined chapters (_nodes_) using the `Enter`/`Return` key. You can go back to the previous node with `p` or read the next node in the guide by pressing `n`. To return to the previous level up in the hierarchy of nodes, press `u`. To quit `info` just press `q`.

## Help from the community

You can also get community-sourced help using a service like [Cheat.sh](https://cheat.sh). This works well with the `curl` command, which fetches online information and prints it to standard output.

To see examples of how to use the `tar` command, for instance, you just need to point curl to `cheat.sh/` and add `tar` at the end of the URL. This also works to get help on specific topics in many programming languages (like Python) -- just use an extra slash before the topic:

```bash
curl cheat.sh/tar # examples of using the tar command
curl cheat.sh/python/split # information about the split method in Python
curl cheat.sh # usage info
```
