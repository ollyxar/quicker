# Quicker: Fast Docker Dev Env

![quicker](https://i.imgur.com/fh5b4sD.png)

This project dedicated for PHP artisans. In the scope we combined most popular stack: **NGINX + PHP7.2 + MySQL**

### Requirements:

* Docker
* Docker-compose

### Configuring:

Most common configuration parameters elevated to main `.env` file. Just rename (copy) `.env.example` file to `.env` and set needed properties.

If you need to install additional features / modules you can specify them in the related `Dockerfile` instructions.

It is convenient to put docker-folder inside the project to get ability to start environment within project. 

### Basics

#### 1. Building (rebuilding)

```bash
docker-compose build
```

#### 2. Starting environment

Please use IDE (PHPStorm) to start environment!

Also it is possible to use command line:
```bash
docker-compose up -d
```

#### 3. Stopping environment

Please use IDE (PHPStorm) to stop environment!

Also it is possible to use command line:
```bash
docker-compose down --remove-orphans
```

#### 4. Attaching to running container

Please use IDE (PHPStorm) to exec bash inside the container!

Also it is possible to use command line:
```bash
docker exec -it quicker-php-fpm su -s /bin/bash www-data
```

