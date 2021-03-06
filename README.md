# mediawiki-php-fpm5.6

This is PHP5.6-FPM for legacy Mediawiki instance.

It's recommended update Mediawiki to latest version and use official Mediawiki container.

## Deploy

Example `docker-compose.yml` file for deployments.

```
version: "3"
services:
  php-fpm:
    image: olkitu/mediawiki-php-fpm5.6
    ports:
    - 127.0.0.1:9001:9000
    volumes:
    - /var/www/html:/var/www/html
    network_mode: bridge
```