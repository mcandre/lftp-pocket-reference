# Troubleshooting

## Caching

By default, LFTP caches directory listings, causing remote `ls` to lag behind file system changes. To fix this, run `cache flush`, or write `set cache:enable no` in your `$HOME/.lftprc` configuration file.

## Rate limit

Run

```
> set net:limit-total-rate <max bytes/sec>
```

Or

```
> set net:limit-total-rate <max bytes/sec (download)>:<max bytes/sec (upload)>
```

before beginning transfers. Optionally, write the command in `$HOME/.lftprc` to remember the setting for future connections.

## Bookmark tab completion

To tab-complete LFTP bookmark names in bash, see https://github.com/mcandre/lftp-completion.