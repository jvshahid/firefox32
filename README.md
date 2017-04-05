# firefox32

A 32 bit firefox docker image/file. to be used with webex

## Building locally

`docker build -t firefox32 .`

## Using prebuilt image

`docker pull jvshahid/firefox32`

## Running

Enable connections to your X11 server

`xhost +`

Then,

`docker run -v /tmp/.X11-unix/X0:/tmp/.X11-unix/X0 -it bash -l`

once running a shell in the container, start firefox:

`$ firefox`

**note** firefox might crash the first time you start it up. Just hit the `Restart Firefox` button. I still haven't figured out why that's the case
