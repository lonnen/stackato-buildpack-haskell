# Stackato Buildpack: Haskell

This is a [buildpack](http://devcenter.heroku.com/articles/buildpacks)
for Haskell apps inteded to be used with Stackato. It uses GHC 7.4.1 and cabal-1.16.0.1.

This requires a few additional system packages to get Cabal to build.

Doesn't work too well with Heroku since it relies on stackato's ability to install system packages

```
env:
    BUILDPACK_URL: https://github.com/lonnen/stackato-buildpack-haskell
requirements:
    ubuntu:
        - libgmp3c2
        - libgmp3-dev
        - freeglut3
        - freeglut3-dev
        - haskell-platform

```
