# docker-laravel-nginx
An image to serve a laravel app with nginx

### How to use

- Mount your Laravel app in `/var/www/html/`
- Expose the port `80`

`docker run -d -p 8080:80 -v /path/to/laravel:/var/www/html ollaapp/laravel-nginx`
