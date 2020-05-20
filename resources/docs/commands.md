# Laravel instalation
sudo chmod 0777 -R storage/
php artisan key:generate

# Instaling Nova
php artisan nova:install

## creating a user
php artisan nova:user

## migrations
php artisan make:migration create_posts_table
php artisan make:migration --table=posts add_more_post_columns

## making the models
php artisan make:model Post

## making the resources
php artisan nova:resource Post