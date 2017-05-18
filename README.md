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

`docker run --rm -v /tmp/.X11-unix/X0:/tmp/.X11-unix/X0 jvshahid/firefox32`
