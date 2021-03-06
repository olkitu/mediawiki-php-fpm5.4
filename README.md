# mediawiki-php-fpm5.4

This is PHP5.4-FPM for legacy Mediawiki 1.20.

It's recommended update Mediawiki to latest version and use official Mediawiki container.

## Deploy

Example `docker-compose.yml` file for deployments.

```
version: "3"
services:
  php-fpm:
    image: olkitu/mediawiki-php-fpm5.4
    ports:
    - 127.0.0.1:9000:9000
    volumes:
    - /var/www/html:/var/www/html
    network_mode: bridge
```