# IntelliJ CE Inside Docker

[![](https://badge.imagelayers.io/smilingrob/intellij-ce:latest.svg)](https://imagelayers.io/?images=smilingrob/intellij-ce:latest 'Get your own badge on imagelayers.io')

Run IntelliJ Idea Community Edition 15.0.4 inside a docker container.
This version runs with Open JDK 8 installed.

## Running

```bash
docker run -dti -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix \
           -v $HOME/dev:/home/developer/dev \
           --name idea smilingrob/intellij-ce
```

Assuming you put your source in a folder in your home called `~/dev/`, you might want to change it for your particular use case.
Docker will start the container with a new user called `developer` and it's `/home/developer/dev` will mirror your `~/dev`

