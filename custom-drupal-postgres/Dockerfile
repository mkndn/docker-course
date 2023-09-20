# create your custom drupal image here, based of official drupal

FROM drupal:10-apache-bullseye

RUN apt-get update && apt-get install -y git \
&& rm -rf /var/lib/apt/lists/*

WORKDIR /var/www/html/themes

RUN git clone https://git.drupalcode.org/project/gin.git \
&& chown -R www-data:www-data gin


WORKDIR /var/www/html
