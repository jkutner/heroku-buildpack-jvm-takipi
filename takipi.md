# Takipi

### Table of Contents
- [Introduction](#introduction)
- [Supported languages & frameworks](supported-languages--frameworks)
- [Install](#install)
- [Use](#use)

#### Introduction

[Takipi](https://addons.heroku.com/takipi) can be installed as an Heroku [Add-On](https://addons.heroku.com).
Once installed on your app, Takipi will detect events (such as exceptions or breakpoint hits) happening within your app and automatically create the code needed to log and collect the data you'll need to debug these events in production.

All the information will be available in the [Takipi webapp](https://app.takipi.com).
Log in throguh the add-on Single Sign On or [create an account](https://app.takipi.com/account.html)

Once logged-in you will need to specify the installation unique key, used to encrypt your data.
The key is sent to the owner of the app when installing / downloaded when creating an account in Takipi website.

If you are an existing Takipi user, you can use `heroku config:set TAKIPI_MACHINE_KEY=S1...` to reuse your key.

#### Supported languages & frameworks
We support OpenJDK and HotSpot versions 6 and 7 (64bit only).

We support all JVM languages. Java, Scala, Clojure, JRuby, etc...

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
