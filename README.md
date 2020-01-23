# Dockerized PHP

[Documentation](https://dockerfile.readthedocs.io/en/latest/content/DockerImages/dockerfiles/php-dev.html)

## Requirements

- docker (min 17.03.1-ce)
- docker-compose (min 1.13.0)

## Installation

Create `.env` from example `.env.dist`, if you prefer different parameters like port or PHP version.

```shell script
chmod +x ops
./ops up
```

## Stop
```shell script
./ops down
```

## Useful commands

```shell script
# run PHP file
./ops php index.php

# get composer version
./ops bash composer --version

# start PHP built-in webserver, now you can open `localhost` on `PHP_SERVER_PORT` in browser,
# by default it is: http://localhost:9001
./ops php -S 0.0.0.0:9001
```