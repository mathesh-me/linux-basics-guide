## Shell Types

### Types of Shells

Commonly types of shells in Linux:
- **Bourne Shell (sh):** It is the oldest shell and is the default shell in Unix-like systems.
- **Bourne Again Shell (bash):** It is the most widely used shell in Linux. It is the default shell in most Linux distributions.
- **C Shell (csh):** It is a shell that was developed at the University of California, Berkeley.
- **Korn Shell (ksh):** It is a shell that was developed by David Korn at Bell Labs.
- **Z Shell (zsh):** It is a shell that is an extended version of the Bourne Shell (bash).
- **Fish Shell (fish):** It is a shell that is designed to be user-friendly and interactive.

### Changing the Shell

We can change the shell by using the `chsh` command.
```bash
chsh -s /path/to/shell username
```
The above will prompt for the password of the user and then change the shell to the specified shell.

### Aliases

Aliases are like a shortcut for commands. We can set aliases using the `alias` command. 

```bash
alias alias_name='command'
```

### Shell Variables

Shell variables are used to store information that can be used by the shell. We can set shell variables using the `=` operator. The syntax to set a shell variable is:

```bash
variable_name=value
```
if we using this Command it will only available in the current shell session. Not available to any process or program that is running in the shell.

### Environment Variables

Environment variables are variables that make variables available to all the processes that are running in the shell. We can set environment variables using the `export` command.

```bash
export variable_name=value
```
To make the environment variable permanent, we can add it to the `.bashrc`, `.bash_profile`, or `.profile` file.

```bash
echo "export variable_name=value" >> ~/.bashrc
```

### Path Variable

The `PATH` variable is an environment variable that stores a list of directories where the shell looks for executable files. When we run a command in the shell, the shell searches for the command in the directories listed in the `PATH` variable. We can add a directory to the `PATH` variable using the `export` command.

```bash
export PATH=$PATH:/path/to/directory
```
To find the path of a command, we can use the `which` command.

```bash
which command
```
### Bash Prompt

The Bash prompt is the text that is displayed in the shell. The Bash prompt can be customized by setting the `PS1` variable. The `PS1` variable is used to set the primary prompt string. We can set the `PS1` variable in the `.bashrc` file. The default value of the `PS1` variable is:

```bash
export PS1="\u@\h:\w\$ "
```

#### Customizing the Bash Prompt

We can customize the Bash prompt by setting the `PS1` variable. Some of the common escape sequences that can be used in the `PS1` variable are:

**Most Common Escape Sequences:**

- `\u` - username of the current user
- `\h` - hostname of the machine
- `\w` - current working directory
- `\W` - basename of the current working directory
- `\d` - date in "Weekday Month Date" format
- `\t` - current time in 24-hour HH:MM:SS format