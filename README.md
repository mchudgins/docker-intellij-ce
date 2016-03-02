# IntelliJ CE Inside Docker

## Installation

```bash
docker build -t idea .
```

## Running

```bash
./idea
```

The `idea` bash script assumes you put your dev source in a folder in your home called `~/dev/`, you might want to change it for your particular use case.
Docker will start the container with a new user called `developer` and it's `/home/developer/dev` will mirror your `~/dev`
