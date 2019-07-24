FROM ubuntu:latest
MAINTAINER Justin Roysdon
# Original concept taken from Scott Lowe https://github.com/scottslowe/dockerfiles and aliustaoglu/firefox
# On Linux, docker run --rm -e DISPLAY=yourIPAddressHere:0 -v /tmp/.X11-unix:/tmp/.X11-unix -it firefox-ubuntu
# On MacOS, you need to install XQuartz.org, then run the docker run above

RUN apt-get -y update && apt-get -y install firefox --no-install-recommends && \
    rm -rf /var/lib/apt/lists*

ENTRYPOINT [ "/usr/bin/firefox" ]
