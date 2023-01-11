# Yet Another NUS Sync

Shell script to sync your files from NUS Canvas.

Only files available through Canvas API are downloaded; externals in-text links and readings are not supported.

> yans -k "\$(pass show canvas-api)" ~/nus

By default, the files will not be overwritten, unless the option `--clobber` or `-c` is passed. E.g.,

> yans --clobber -k "\$(pass show canvas-api)" ~/nus

## Dependencies

- `wget`
- `curl`
- `jq`
