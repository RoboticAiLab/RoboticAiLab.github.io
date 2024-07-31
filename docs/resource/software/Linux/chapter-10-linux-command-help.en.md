---
comments: true
---

# Chapter 10: Getting Help in Linux Terminal

Learn how you can get help about using Linux commands in the final chapter of the Terminal Basics series.

These days, you can search the internet for the usage and examples of any command.

But it was not like this when the internet didn't exist, or it was not as widely available to everyone.

For this reason, commands in Linux (and the operating systems before it) come with a help or manual page (man pages). This worked as a reference and users could access it anytime to see what options were available for a command and how it worked.

The man pages are still relevant in this age of information abundance.

First, they are the original command documentation and hence the most trusted source on command usage.

Second, if you are taking some Linux exam, you will not be allowed to search on the internet but the man pages are always at your disposal.

Now that you understand the importance of getting help directly in the terminal, let's see more about them.

## Get help with Linux commands in the terminal

There are two main commands to get help on the usage of a Linux command:

- help: For shell builtin commands
- man: For other Linux commands

### Wait! What are shell built-in commands?

You may feel that commands like ls, rm, mv are part of the bash shell. But that's not true. Shell only has a few commands that are built into it as a part of the shell itself. This is why they are called built-in commands. Some examples of built-in commands are echo, cd, and alias.

Other popular Linux commands like ls, mv, rm, cat, less, etc are part of a software package called [GNU coreutils](https://www.gnu.org/software/coreutils/?ref=itsfoss.com). They come preinstalled on almost all Linux distributions.

You won't find man pages for the shell built-ins.

```
abhishek@tuxedo:~$ man cd
No manual entry for cd
```

The man pages are for these 'external' Linux commands. The shell built-ins have help sections.

💡

Want to see all the built-in shell commands? Just type `help` to list them all.

### Use man to see command documentation

Using the man command is simple. Just give it command's name like this:

```
man command_name
```

And it will open the manual page of the command. You'll find the syntax of the command, its options, and a brief explanation of the options.

[![An example manpage of the ip command in Linux](https://itsfoss.com/content/images/2023/04/man-page-example.png)](https://itsfoss.com/content/images/2023/04/man-page-example.png)

The pages are (usually) [opened with the less command](https://itsfoss.com/view-file-contents/) so you can use all the [keyboard shortcuts of the less command](https://linuxhandbook.com/less-command/?ref=itsfoss.com) to move around and search for text.

Don't remember it? This will help you recall

| **Keys**      | **Action**                                         |
| ------------- | -------------------------------------------------- |
| Up arrow      | Move one line up                                   |
| Down arrow    | Move one line down                                 |
| Space or PgDn | Move one page down                                 |
| b or PgUp     | Move one page up                                   |
| g             | Move to the beginning of the file                  |
| G             | Move to the end of the file                        |
| ng            | Move to the nth line                               |
| /pattern      | Search for pattern and use n to move to next match |
| q             | Exit                                               |

There is more to man pages than. I cannot cover it all here, but we do have a detailed guide. Feel free to refer to it.

[RTFM! How to Read (and Understand) the Fantastic Man Pages in Linux](https://itsfoss.com/linux-man-page-guide/)

### Use help command for shell built-ins

As mentioned earlier, no man pages exist for the built-in shell commands. Instead, you use the help command like this:

```
help command_name
```

It will show a summary of the command options. The entire content is displayed on the screen, unlike the man command.

[![Using help for built-in shell commands](https://itsfoss.com/content/images/2023/04/help-for-shell-built-ins.png)](https://itsfoss.com/content/images/2023/04/help-for-shell-built-ins.png)

### Help option for all commands

Do you feel the man page has too much information and you just want to see the options of a command? The help option 'helps' you.

Almost all Linux commands provide a `--help` option that should summarize the available options.

[![Using help option of Linux commands](https://itsfoss.com/content/images/2023/04/help-with-linux-commands.png)](https://itsfoss.com/content/images/2023/04/help-with-linux-commands.png)

However, it's not a hard and fast rule. The help sections of some commands are pretty bland. Try it for the ip command.

## There are more ways to get help in Linux terminal

There is the info command that works similar to the man command.

If you find man pages complicated to understand, there are third-party tools that simplify the content of man pages and make it more beginner friendly. TLDR is one such package you can use.

[TLDR: Linux Man Pages Simplified](https://itsfoss.com/tldr-linux-man-pages-simplified/)

In other words, the help is just a few key presses away.

It's not that only new Linux users need help. Experienced Linux users specially rely on the manpages. So don't shy away from using the help in the terminal.

I also advise [using the history command](https://linuxhandbook.com/bash-history-tips/?ref=itsfoss.com). This way, you can search for the commands you typed earlier.

[5 Simple Bash History Tricks Every Linux User Should Know](https://linuxhandbook.com/bash-history-tips/?ref=itsfoss.com)

## This is the end... or the beginning

And with this, I conclude the Linux Terminal Basics series.

In the ten chapters of the series, you got familiar with the terminal, learned to move around in the terminal, and create, move and delete files and folders. You also learned to read and edit files.

This gives you a basic but solid foundation of Linux commands. It may be the end of this series, but it helps begin your Linux command line journey.

You'll find more in-depth guides on 'doing things in Linux command line' on It's FOSS in the future. It may not be in a series (or maybe it will) but you'll have plenty of opportunity for learning.

💬 ***I hope you liked this beginner series. I welcome your feedback on the usability of this series and suggestions to improve it. If you have any suggestions for a related new series, please don't hesitate. The comment section is waiting for you.\***
