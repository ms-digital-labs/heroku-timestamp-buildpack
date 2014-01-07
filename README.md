#Heroku Release Timestamp Buildpack

You know when you're not entirely sure what code heroku is running? Maybe you're using the preboot labs feature? Maybe you got drunk and blacked out with your hand over the deploy button? Maybe you're just curious?

This buildpack will put a `release.txt` file in the public directory of your app on deploy, and fill it with the current date/time.

It is intended to be used with the [multi buildpack buildpack](https://github.com/ddollar/heroku-buildpack-multi) (because otherwise it's pointless).

We'd also like to include the git commit hash, but we don't seem to be able to get hold of it from within the slug compilation environment.