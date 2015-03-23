# Troubleshooting

## Caching

By default, LFTP caches directory listings, causing LFTP `ls` to lag behind file system changes, as files are created, deleted, or moved. To fix this, run `cache flush`, or write `set cache:enable no` in your `$HOME/.lftprc` configuration file.

## Rate limit

Run

```
> set net:limit-total-rate <max bytes/sec>
```

Or

```
> set net:limit-total-rate <max bytes/sec (download)>:<max bytes/sec (upload)>
```

before beginning transfers. Optionally, write these commands in `$HOME/.lftprc` to remember the setting for future connections.

## Bookmark tab completion

To tab-complete LFTP bookmark names in bash, see https://github.com/mcandre/lftp-completion.