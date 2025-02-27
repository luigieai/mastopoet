# Mastopoet

The Toot screenshot tool for Mastodon. Developed by [@raikas@mementomori.social](https://mementomori.social/@raikas)

## What?

Mastopoet is an open source screenshot tool for [Mastodon](https://joinmastodon.org), inspired by [poet.so](https://poet.so).
It allows you to create ✨ stunning ✨ screenshots of your toots, with ability to remove stuff you don't want (bookmark button, publicity symbol, settings button...). And with a theme that's not dependent on the theme of the instance!

## Demo

[mastopoet.ohjelmoi.fi](https://mastopoet.ohjelmoi.fi)

## URL Query feature

Add ?url=<toot url> to the end of the Mastopoet URL to generate links that immediately open the toot on Mastopoet.

## Themes available

- [Bird UI](https://github.com/ronilaukkarinen/mastodon-bird-ui) (Dark, Light)
- Mastodon (Dark, Dark + light interaction labels, Light)

## TODO

- [x] Customizable gradient
- [x] Bird UI light theme port
- [x] Mastodon theme port
- [ ] Customizable date format
- [ ] A logo (to website embed)
- [x] Read toot URL from query
- [x] Default Toot with information
- [ ] Fix multi image image galleries
- [ ] Support for non-mastodon links
- [ ] Alt text generator

## Building with docker
You can use docker for deploying a production ready instance of Mastopoet. 

You can build with:
```console
docker build -t mastopoet .
```
It will build the application and deploy in a nginx instance, when the image is builded you can run using:
```console
docker run -d -p 80:80 mastopoet
```
For more options, see [nginx container options at dockerhub](https://hub.docker.com/_/nginx).
## Credits

- [Mastodon Bird UI](https://github.com/ronilaukkarinen/mastodon-bird-ui/) by Roni Laukkarinen, licensed under MIT
- [Mastodon](https://github.com/mastodon/mastodon)
- [Tabler Icons](https://tabler-icons.io), linced under MIT
