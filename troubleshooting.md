# Troubleshooting

## Caching

By default, LFTP caches directory listings. Therefore, LFTP `ls` may lag behind file system changes, as files are created, deleted, or moved. To fix this, run `cache flush`, or write `set cache:enable no` in your `$HOME/.lftprc` configuration file.