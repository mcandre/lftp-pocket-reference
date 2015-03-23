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

## Download a single file

```
> get <path>
```

E.g.:

```
> get index.html
```

## Download a single file faster, in parallel segments

```
> pget <path>
...
```

E.g.,:

```
> pget index.html
ooo
```

## Upload a single file

```
> put <path>
```

## Download a directory

```
> mirror <path>
```

## Upload a directory

```
> mirror -R <local path> <remote path>
```

## Caching

By default, LFTP caches directory listings; if a file or folder is created, deleted, or moved, LFTP `ls` may not reflect the change. To fix this, run `cache flush`, or write `set cache:enable no` in your `$HOME/.lftprc` configuration file.