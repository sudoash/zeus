# Zeus

Zeus is a utility wrapper for Docker on macOS / OS X. It combines [docker](https://docs.docker.com), [docker-compose](https://docs.docker.com/compose/), [docker-machine](https://docs.docker.com/machine/) and [docker-machine-nfs](https://github.com/adlogix/docker-machine-nfs).

## Requirements

  - Docker
  - Docker Compose
  - Docker Machine
  - Docker Machine NFS

## Installation

### Homebrew

```
brew install sudoash/tap/zeus
```

### Standalone

Download the [zeus](https://raw.githubusercontent.com/sudoash/zeus/master/zeus) bash script and put in your `$PATH`.

## Getting started

Before you can use Zeus, you need to create a `Zeusfile`. The easiest way to create one is by using `zeus init`. You should end up with something like this:

```
# Automatically generated by zeus
ZEUS_NAME=local
ZEUS_DOMAIN=local.dev

# The default shell to run when SSH'ing into the container
ZEUS_SHELL=bash

# The default container to SSH into when running zeus ssh with no container argument
#ZEUS_DEFAULT_SSH_CONTAINER=
```

## Usage
```
zeus - the utility wrapper for docker, docker-compose, docker-machine and docker-machine-nfs
zeus version 0.5

Usage: /usr/local/bin/zeus <command>

Commands:
  init             Initialises Zeus and creates a Zeusfile
  create           Creates the Docker machine for the first time
  up               Starts the Docker containers
  down             Removes the Docker containers
  reload           Recreates the Docker containers
  list             Lists Docker containers
  ssh [container]  Connect via SSH to the specified container
  info             Displays info for your Docker machine
  destroy          Removes the Docker machine
  fix              Attempts to fix any SSL or NFS issues
 ```

## Todos

 - Multiple docker-machine drivers
 - Linux support
 - Autocomplete commands

## Credits

Thanks to the guys behind these amazing Docker tools!

## License

MIT License
