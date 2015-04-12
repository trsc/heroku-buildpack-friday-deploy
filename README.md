Friday Deploy Buildpack *
=========================
(* Saturday and Sunday support included)

## Why?
Of course no sane person should attempt a deploy on a Friday! Of course! But sometimes we have to be brave souls and do what we shouldn't. This "buildpack" will at least let you know it's not the greatest plan!

The idea for this project was incepted by a [tweet](https://twitter.com/yurykusik/status/556064634525204481). There is a [Capistrano recipe](https://github.com/marshall-lee/capistrano-friday) available, but none for Heroku or compatible deployment scenarios, until now.

## What you get
Depending on the week day you may see something like this:
```
-----> Multipack app detected
       =====> Downloading Buildpack: https://github.com/trsc/heroku-buildpack-friday-deploy
       =====> Detected Framework: Friday Deploy
-----> so you decided to take the plunge?
       ┓┏┓┏┓┃
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃
       ┛┗┛┗┛┃ ⟍ ○⟋
       ┓┏┓┏┓┃   ∕
       ┛┗┛┗┛┃ ノ)
       ┓┏┓┏┓┃          Friday
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃          deploy,
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃          good
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃          luck!
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃
       ┛┗┛┗┛┃
       ┓┏┓┏┓┃
       ┃┃┃┃┃┃
       ┻┻┻┻┻┻
```

## How to use it
* Create a `.buildpacks` file with the following content
```
https://github.com/trsc/heroku-buildpack-friday-deploy
https://github.com/heroku/heroku-buildpack-scala
```
* Replace the 2nd line with the builpack required by your application, the example uses the buildpack for Scala
