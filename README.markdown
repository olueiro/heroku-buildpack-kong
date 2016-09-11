[Heroku Buildpack](https://devcenter.heroku.com/articles/buildpacks) for [LuaJIT](https://luajit.org)
=========================
Supports [LuaRocks](http://luarocks.org)

_Alpha_

Usage
-----

* Add this buildpack in your Heroku project
* You can add LuaRocks modules to build on deploy your project:
  Create a file named *.luarocks*; each line is `{LUARCOKS MODULE NAME}`

### Environment variables

  * `PORT` exposed on the app/dyno
    * set automatically by the Heroku dyno manager

Modification
------------
This buildpack caches its compilation artifacts from the sources in `vendor/`. Changes to the sources in `vendor/` will be detected and the cache ignored.
