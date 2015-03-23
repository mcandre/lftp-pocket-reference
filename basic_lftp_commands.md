# Basic LFTP Commands

## Connect to server

`lftp` opens an FTP session, and then prompts for more LFTP commands.

```
$ lftp <URL>
> (other LFTP commands...)
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

## Quit / Disconnect from server

```
> quit
```

Or press `Control+D` (Unix) / `Control+C` (Windows).