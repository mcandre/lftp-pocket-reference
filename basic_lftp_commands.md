# Basic LFTP Commands

## Connect to server

`lftp` opens an FTP session, and then prompts for more LFTP commands.

```
$ lftp <URL>
> (other LFTP commands...)
```

E.g., `lftp ftp://ftp.hq.nasa.gov/`

## Create a bookmark

If you frequently connect to the same FTP server, you may want to create an LFTP bookmark to make it easier to access.

```
> bookmark <name>
```

E.g., `bookmark nasa`

Now, you don't have to remember the full FTP URL anymore!

## Connect to bookmarked server

```
$ lftp <name>
```

E.g., `lftp nasa`

Tab-completion for LFTP bookmarks can be setup with [lftp-completion](https://github.com/mcandre/lftp-completion).

## Quit / Disconnect from server

```
> quit
```

Or press `Control+D` (Unix) / `Control+C` (Windows).

## Navigation

Graphical FTP clients tend to offer a side-by-side view of local vs. remote files. LFTP presents all this information in one view, using distinct commands for referring to local vs. remote files. LFTP tends to use Unix-style commands for remote files, and prefix these commands with `l` for local files.

### Change remote directory

Like SSH, LFTP has a temporary concept of where the user is with respect to the remote directory tree.

```
> cd <directory>
```

### Change local directory

```
> lcd <directory>
```