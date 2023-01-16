# Docker for PHP5.6
Docker setup for running your old php projects

## How To
```sh
# Grant Permission
chmod +x build.sh run.sh

# Buld the Image
./build.sh

# Run the php
./run.sh
```

Your server will start on http://localhost/8099

### Configuration
Below is the description docker run script
```sh
docker run -d --rm -p 8089:80 -v /home/ayopop/Documents/docker-php5:/var/www/html ax/php56:latest

# docker run -d -rm -p [host-port]:[container-port] -v [host-www-html-dir]:[mount-in-container] [image-name]:[version]
```

### Thanks
Script from https://hub.docker.com/r/porchn/php5.6-apache/dockerfile