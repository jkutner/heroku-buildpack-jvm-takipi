# Takipi

### Table of Contents
- [Introduction](#introduction)
- [Supported languages & frameworks](supported-languages--frameworks)
- [Install](#install)
- [Use](#use)

#### Introduction

Takipi - Server debugging made easy

#### Supported languages & frameworks
We support OpenJDK and HotSpot versions 6 and 7 (64bit only).

We support all JVM languages. Java, Scala, Clojure, etc...

#### Install

Installing Takipi is super easy!

You will need to setup the [Heroku Takipi Buildpack](https://github.com/takipi/heroku-buildpack-jvm-takipi) in your app.

In order to use this buildpack enter the directory of your app.

For a new app run:

`heroku create myapp --buildpack https://github.com/takipi/heroku-buildpack-jvm-takipi.git`

Or for a running app run:

`heroku config:set BUILDPACK_URL=https://github.com/takipi/heroku-buildpack-jvm-takipi.git`

#### Use

Follow our [getting started guide](http://www.takipi.com/starting.html?nav=guide).


By [Takipi, Inc.](http://www.takipi.com) 2013. Contact us: hello@takipi.com
