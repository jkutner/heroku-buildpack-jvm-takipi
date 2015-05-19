# heroku-buildpack-jvm-takipi

Creating a cedar stack application with this buildpack will install Takipi alonside the default
JVM specific language needed to run your application. We support the [Java](https://github.com/heroku/heroku-buildpack-java),
[Scala](https://github.com/heroku/heroku-buildpack-scala), [Clojure](https://github.com/heroku/heroku-buildpack-clojure),
[Gradle](https://github.com/heroku/heroku-buildpack-gradle), [Grails](https://github.com/heroku/heroku-buildpack-grails)
 and [Play!](https://github.com/heroku/heroku-buildpack-play) default buildpacks.

### Install Takipi

In order to use this buildpack enter the directory of your app.

For a new app run:

`heroku create myapp --buildpack https://github.com/takipi/heroku-buildpack-jvm-takipi.git`

Or for a running app run:

`heroku buildpacks:set https://github.com/takipi/heroku-buildpack-jvm-takipi.git`

### Setup Takipi

Once your app is configured to run Takipi, either add [Takipi addon](https://addons.heroku.com/takipi) or setup Takipi manually:

1. Create an account at https://app.takipi.com/account.html
2. Run `heroku config:set TAKIPI_SECRET_KEY=S193#...` with the key received in step 1.
 
#### Have fun and enjoy
