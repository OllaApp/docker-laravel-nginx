# docker-laravel-nginx
An image to serve a laravel app with nginx

### How to use

Extend this image with a Dockerfile

- Copy your laravel app to `/var/www/html`
- Run composer install

```Dockerfile
FROM ollaapp/laravel-nginx

COPY ./my-laravel-app /var/www/html

RUN composer install && \
    chown -R www-data/www-data /var/www/html
```

Nginx is served on the port `80`
