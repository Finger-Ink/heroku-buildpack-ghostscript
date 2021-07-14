# Heroku Buildpack for Ghostscript

## Currently installs Ghostscript 9.54.0 on Heroku Cedar.

#### Install

```shell
$ cd /path/to/your-app
$ heroku buildpacks:add https://github.com/Wilfison/heroku-buildpack-ghostscript.git

# Push changes to deploy
$ git push heroku master

# This version of ghostscript will end up deployed at /app/vendor/gs/bin/gs
# So you may want to set an environment variable to let your app know where it is. e.g.
$ heroku config:set GS_PATH=/app/vendor/gs/bin/gs
```
