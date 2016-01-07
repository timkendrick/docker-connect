# docker-connect
> Local Docker machine launcher

`docker-connect` allows you to connect to your local Docker machines with one quick and easy command, and cleans up after itself once you're done.

## Usage

```bash
docker-connect [machine=default]
```

This will perform the following steps:

1. Start the Docker machine specified by the `machine` argument (default: `"default"`)
2. SSH into the Docker machine
3. Once the SSH session has exited, suspend the VirtualBox machine for reuse


## Installation

```
git clone https://github.com/timkendrick/docker-connect /usr/local/lib/docker-connect
ln -s ../lib/docker-connect/docker-connect /usr/local/bin/docker-connect
```


## System requirements

- Mac OS X
- [Docker Toolbox](https://www.docker.com/docker-toolbox)