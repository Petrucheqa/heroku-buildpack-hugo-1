# Heroku Buildpack: Hugo

This is a Heroku Buildpack for [Hugo blog engine](https://gohugo.io/) with support for syntax highlighting with [Pygments](http://pygments.org/) (a Python package).

To use this buildpack you will need a Hugo website with a config file in one of the expected formats (config.toml, config.yaml or config.json) in the root directory.

To use Pygments for syntax highlighting you will need to include a `requirements.txt` in the root directory, with the Pygments version you wish to include, like this:

    pygments==2.1.1

I have built this buildpack on top of the

* [Python Buildpack](https://github.com/heroku/heroku-buildpack-python)

with some inspiration from these two GitHub repos:

* [roperzh/heroku-buildpack-hugo](https://github.com/roperzh/heroku-buildpack-hugo)
* [dvdsgl/heroku-buildpack-python-hugo](https://github.com/dvdsgl/heroku-buildpack-python-hugo)

For more information on how to use this buildpack, have a look at [Using a Custom Buildpack](https://devcenter.heroku.com/articles/buildpacks#using-a-custom-buildpack).
