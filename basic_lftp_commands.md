# Basic LFTP Commands

## Connect to server

`lftp` opens an FTP session, and then prompts for more LFTP commands.

```
$ lftp <URL>
> <LFTP commands...>
```

E.g., `lftp ftp://ftp.hq.nasa.gov/`

## Create a bookmark

```
> bookmark <name>
```

E.g., `bookmark nasa`

## Connect to bookmarked server

```
$ lftp <name>
```

E.g., `lftp nasa`

### LFTP Bookmark tab completion

See https://github.com/mcandre/lftp-completion

## Quit / Disconnect from server

```
> quit
```

Or press `Control+D` (Unix) / `Control+C` (Windows).

## Download a file

```
> get <path>
```

E.g.:

```
> get index.html
```

## Download a file faster, in parallel segments

```
> pget <path>
...
```

E.g.,:

```
> pget index.html
ooo
```

## Upload a file

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