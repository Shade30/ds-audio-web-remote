# Web Remote for Synology DS audio

## Setup

Copy into `/usr/syno/synoman/webman/3rdparty/WebRemote/`

Browse `http://<HOST>/webman/3rdparty/WebRemote/music.html`

## Features

- Play/pause, next, prev, stop.
- Clear playlist.
- Load playlist 1-4 (plays personal playlist called "1", "2", "3" or "4", they must be created beforehand)
- Play Random100
- Get current track title and some other data

## Notes

- Remote requires DSM 4.x. Script rewriting is required to make it play to make it compatible to DSM 3.x because request paths are different.
- Remote only plays to USB target. Script rewriting is required to make it play to the Media Renderer.
- Remote needs to re-login periodically, because it is not sending avoid_timeout requests.
- I took first mobile optimized template for WebRemote that I found on the web, so the design is not very optimal for the mobile remote control.
