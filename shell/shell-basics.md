## Shell Basics

### What is a shell?

A shell is a program that allows a text=based interaction between the user and the operating system. It takes commands from the keyboard and gives them to the operating system to perform. In olden days, it was the only user interface available on a Unix-like system. Nowadays, we have graphical user interfaces (GUIs) in addition to command line interfaces (CLIs) such as the shell.

### Commands in the shell

A command is a text-based instruction to the shell to perform a specific task. When we run some command it executes a Specific Program to achieve a specific task.

**More about Commands:**

- Commands in the shell take arguments and options.
- Some Commands need arguments to perform a specific task while some commands don't need arguments.
- Arguments are the values that are passed to the command to perform a specific task. **Example:** `echo "Hello World"` Here `Hello World` is an argument.
- Options are the flags that are passed to the command to modify the behavior of the command. **Example:**  `echo -n "Hello World"` Here `-n` is an option.
- Some Commands don't need arguments or options. **Example:** `pwd` command.

### Types of Commands

There are two types of commands in the shell:

1. **Internal Commands:** These are built-in commands that are part of the shell. These commands are executed by the shell itself. **Example:** `cd`, `pwd`, `echo`, `exit`, `history`.

2. **External Commands:** These are commands that are not part of the shell. These commands are separate programs that are stored in the system. **Example:** `ls`, `cat`, `grep`, `awk`, `sed`, `find`.

We can check whether a command is an internal command or an external command by using the `type` command.

```bash
type cd
type ls
```

### Home Directory

The home directory is the directory where the user is placed after logging into the system. It is represented by the `~` symbol. The home directory of the user is `/home/username`. It will be default directory when we open the terminal.