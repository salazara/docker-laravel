# docker-laravel

```
docker run \
--rm \
--workdir /home/workspace \
--mount type=bind,source=$(pwd),target=/home/workspace \
alpine:latest \
/bin/sh -c \
"rm -rf ./docker-laravel \
&& rm -f ./docker-laravel.tar.gz \
&& wget https://github.com/salazara/docker-laravel/archive/refs/tags/v1.tar.gz -O docker-laravel.tar.gz \
&& tar -xvzf ./docker-laravel.tar.gz \
&& rm -f ./docker-laravel.tar.gz \
&& mv ./docker-laravel-1 ./docker-laravel"
```

```
docker exec -it docker_laravel_app /bin/bash
```

```
composer create-project laravel/laravel .
```