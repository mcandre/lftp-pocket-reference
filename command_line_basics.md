# Command line basics

If you have not used command line interfaces frequently, here are a few refreshing sips of how they work.

## Terminals

Web applications run in Web browsers, command line applications run in terminals.

### Mac OS X

Mac users can open `Terminal.app` with `Spotlight -> Terminal`.

### Windows

Windows users can open `Command Prompt` by launching `Start -> Run -> cmd`.

### Linux

Linux distributions often offer a terminal such as `xfce4-terminal`, `gnome-terminal`, `konsole`, or `xterm`. Graphical Linux distributions often provide a global desktop hotkey for launching terminals: `Control+Alt+T`.

## Prompts

Once a terminal is open, the user is prompted to enter syntax for interacting with command line programs. Unix-based OS's tend to provide a dollar sign prompt (`$`), whereas Windows provides a C greater than prompt (`C:\>`). When LFTP is launched, it provides its own greater than prompt (`>`) to distinguish LFTP commands from normal shell commands.

In any case, this is the terminal's way of asking the user to input some commands. For example, the next section instructs the user to type a command into the terminal that will download and install LFTP. This manual uses `monospace` to indicate that text should be copied & pasted, or otherwise input in a terminal in order to be used.

## File operations

Command line shells offer short, memorable commands for interacting with files and folders. Each command should be copied & pasted, manually typed, or otherwise input into a terminal session. Then, press Enter to execute the command.

### Print current working directory

```
$ pwd
```

### List contents

```
$ ls
C:\> dir
```

### Create directory

In command line descriptions, `text` usually indicates text that should be literally typed as shown; hard brackets (`[ ... ]`) indicate an optional value; and angle brackets (`< ... >`) indicate a placeholder than should be chosen by the user, without actually typing any angle brackets.

```
$ mkdir [-p <path/path/path/>]<path>
```

### Create file

```
$ touch <file>
```

### Copy file or directory

```
$ cp <source> <destination>
C:\> copy <source> <destination>
```

### Move file or directory

```
$ mv <source> <destination>
```

E.g.:

```
$ 
```