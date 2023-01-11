# Yet Another NUS Sync

Shell script to sync your files from NUS Canvas.

Canvas [token](https://canvas.nus.edu.sg/profile/settings) can be obtained from your Account > Settings > Approved integrations > New access token. 

Only files available through Canvas API are downloaded; externals in-text links and readings are not supported.

> yans -k "\$(pass show canvas-api)" ~/nus

By default, the files will not be overwritten, unless the option `--clobber` or `-c` is passed. E.g.,

> yans --clobber -k "\$(pass show canvas-api)" ~/nus

## Dependencies

- `wget`
- `curl`
- `jq`
