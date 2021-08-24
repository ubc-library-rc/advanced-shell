---
layout: default
title: Customizing the shell
nav_order: 5
---
# Customizing the shell

## Creating aliases

Common command combinations or pipelines can be turned into shortcuts called _aliases_ to make it easier and faster to use them on the command-line.

For example, you could alias a long string of command options such as `ls -aRghlo` (which prints a detailed recursive list of the current directory contents with human-readable units and without listing owner or group information) as the much shorter and easier-to-remember command `lsa`:

```bash
alias lsa=ls -aRghlo
```

Then whenever you want to get a comprehensive and recursive list of directory contents you can just type `lsa`, rather than needing to remember all of the command-line options for the `ls` command.

For example, to avoid accidentally deleting important files, you can alias the `rm` command to `rm -i`, which prompts before removing any file:

```bash
alias rm=rm -i
```

In the above command, the `rm` command is _replaced_ with `rm -i` so that whenever you type `rm`, you will actually get a prompt instead of deleting the file.

## Sensible defaults

There are quite a large number of tweaks you can make to the default configuration of Bash to make it easier and more productive to work with. Some of these have been collected together in the [Sensible Bash](https://github.com/mrzool/bash-sensible) project.

You don't need to add all of these to your default Bash profile, but it may be helpful to browse through them and perhaps try a few of them out if they seem useful for your workflow.

You can read through the collection of "sane defaults" directly on the command-line using the following command:

```bash
curl https://raw.githubusercontent.com/mrzool/bash-sensible/master/sensible.bash | less
```

To add a particular default to your Bash profile, open your `~/.bashrc` file in a text editor and paste it at the end of the file. You will then need to reload your profile by entering `source ~/.bashrc` (or quitting and restarting Bash).

The other major way to adjust the way the command-line looks and behaves is to configure the Bash prompt. You can do this manually, or use something like [liquidprompt](https://github.com/nojhan/liquidprompt), which has a rich set of options pre-configured.
