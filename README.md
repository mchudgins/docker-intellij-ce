# IntelliJ CE Inside Docker

[![](https://badge.imagelayers.io/smilingrob/intellij-ce:latest.svg)](https://imagelayers.io/?images=smilingrob/intellij-ce:latest 'Get your own badge on imagelayers.io')


## Installation From Source

```bash
docker build -t idea -f Dockerfile-15.0.4 .
```

## Running

```bash
./idea
```

The `idea` bash script assumes you put your dev source in a folder in your home called `~/dev/`, you might want to change it for your particular use case.
Docker will start the container with a new user called `developer` and it's `/home/developer/dev` will mirror your `~/dev`
