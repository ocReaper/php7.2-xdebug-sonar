# PHP 7.2 cli with xdebug and sonar scanner

This image allows you to run and debug your PHP code and the ability to run sonar scanner on your project thanks to Docker.

Installation
---

### Pull from Docker Hub
```
docker pull ocReaper/php7.2-xdebug-sonar
```

### Or build from GitHub
```
docker build -t ocReaper/php7.2-xdebug-sonar github.com/ocReaper/dockerfile-php7.2-xdebug-sonar
```

### Run image
```
docker run -it ocReaper/php7.2-xdebug-sonar bash
```

### Or use as base image
```Dockerfile
FROM ocReaper/php7.2-xdebug-sonar
```

### Or use it with docker-compose
```yml
app:
  image: ocReaper/php7.2-xdebug-sonar
  ports:
    - 9000:9000
  expose:
    - 9000
  environment:
    PHP_XDEBUG_ENABLED: 1
  tty: true
  stdin_open: true
```
