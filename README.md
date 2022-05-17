# php-local-dockers

Setting up dockers for php in development

## Setting up in `php-dockers`

1. Edit `docker-compose.yml` (you can comment `#` phpmyadmin's container if you don't want to use it).
   Change `working_dir` and database `environment`
2. Edit docker-nginx > `default.conf` root's directory `/var/www/project_public`;
3. Checking `Dockerfile` in `docker-php` and `docker-nginx` that you need.

## Docker up

1. run command `docker-compose up -d` until finished.
2. `.gitignore` add path `/php-dockers/mysql` do not push it to git, just keep it in local.
3. You can remove container `local_phpmyadmin` and `local_composer` if you don't want to use it after docker up.
