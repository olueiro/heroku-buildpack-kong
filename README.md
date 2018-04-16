[Heroku Buildpack](https://devcenter.heroku.com/articles/buildpacks) for [LuaJIT](https://luajit.org)
=========================
Supports [LuaRocks](http://luarocks.org)

_Beta_

Usage
-----

* Add this buildpack in your Heroku project
* You can add LuaRocks modules to build on deploy your project:
  Create a file named *.luarocks*; use a space to separate LuaRocks modules e.g. `lapis pgmoon`

### Environment variables

  * `PORT` exposed on the app/dyno
    * set automatically by the Heroku dyno manager
    * Lua sample `os.getenv("PORT")`
