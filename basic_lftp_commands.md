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

Graphical FTP clients tend to offer a side-by-side view of local vs. remote files. LFTP presents all this information in one view, using distinct commands for referring to local vs. remote files. LFTP uses Unix-style commands for remote files, and tends to prefix these commands with `l` for local files.

### Print working directory (remote)

Like SSH, LFTP has a temporary concept of where the user is with respect to the remote directory tree.

```
> pwd
```

E.g.:

```
> pwd
ftp://ftp.hq.nasa.gov/
```

### Print working directory (local)

```
> lpwd
/Users/mcandre
```

### List files (remote)

```
> ls
```

E.g.:

```
> ls
README
armd
chmgt
ftp-exec
incoming
index.html
lost+found
office
pub
robots.txt
```

### List files (local)

```
> local ls
```

### Change directory (remote)

```
> cd <directory>
```

E.g.:

```
> cd pub
> pwd
ftp://ftp.hq.nasa.gov/pub
```

### Change directory (local)

```
> lcd <directory>
```

E.g.:

```
> lcd Desktop
> lpwd
/Users/mcandre/Desktop
```