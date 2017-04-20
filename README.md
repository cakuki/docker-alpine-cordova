# Docker Alpine Cordova

[![Docker Pulls](https://img.shields.io/docker/pulls/cakuki/alpine-cordova.svg?style=flat-square)](https://hub.docker.com/r/cakuki/alpine-cordova)

Lightweight image to run android builds for Cordova projects.

## Supported tags and respective `Dockerfile` links

* `6.2.1`, `6`, `latest` [(6/Dockerfile)](https://github.com/cakuki/docker-alpine-cordova/blob/master/Dockerfile)


## Usage

Just mount your Cordova project root to `/data` directory and run cordova commands.

```bash
cd <path-to-your-cordova-project>
docker run --rm -v $PWD:/data cakuki/alpine-cordova cordova platform add android
docker run --rm -v $PWD:/data cakuki/alpine-cordova cordova build android
```
