## Run app :
 - docker build -t <project_name> .
 - docker run --rm -it -d -p 80:80  -v $(pwd):/var/www/html --name <project_name> <project_name>
 - In container bash :
   - composer install | chown -R www-data:www-data /var/www/html/storage /var/www/html/bootstrap/cache
   - create .env
   - php artisan key:generate