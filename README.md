# lyrics.ovh: Only the lyrics

Source of the website ~~https://lyrics.ovh~~ (no longer live) which allows you to find the lyrics for a song quickly and without ads.

A Chrome Extension is also available, thanks to Varal7: https://github.com/Varal7/lyrics-chrome-extension.

## API documentation

An API is available to get the lyrics of a song.
The documentation is available on Apiary.io: http://docs.lyricsovh.apiary.io/.

## How to start

```
docker-compose up
```

Finally you can open your browser and access http://localhost:8080 to reach the frontend.

The API endpoints are:

- http://localhost:8080/v1/:artist/:song
- http://localhost:8080/suggest/:term

## Deploy to Heroku

### One-click deployment

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

### Heroku CLI

Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

Create a Heroku app:

```
heroku create
```

Set the app's stack to `container`:

```
heroku stack:set container
```

Deploy:

```
git push heroku master
```
