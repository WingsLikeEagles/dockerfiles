# Run Firefox inside a container and display it via X11 on the local host.
Original concept taken from Scott Lowe https://github.com/scottslowe/dockerfiles and aliustaoglu/firefox

On Linux, docker run --rm -e DISPLAY=yourIPAddressHere:0 -v /tmp/.X11-unix:/tmp/.X11-unix -it firefox-ubuntu
On MacOS, you need to install XQuartz.org, then run the docker run above

https://cuneyt.aliustaoglu.biz/en/running-gui-applications-in-docker-on-windows-linux-mac-hosts/
