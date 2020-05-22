My laravel nova package studies

# Commands used

## Laravel instalation
sudo chmod 0777 -R storage/
php artisan key:generate
composer require laravel/scout
php artisan vendor:publish --provider="Laravel\Scout\ScoutServiceProvider"
composer require algolia/algoliasearch-client-php

## Instaling Nova
php artisan nova:install

## creating a user
php artisan nova:user

## migrations
php artisan make:migration create_posts_table
php artisan make:migration --table=posts add_more_post_columns
php artisan make:migration create_post_tag_table

## making the laravel models
php artisan make:model Post
php artisan make:model Tag


## making the nova resources
php artisan nova:resource Post
php artisan nova:resource Tag


## creating laravel policies
php artisan make:policy PostPolicy -m Post

## creating nova filters
php artisan nova:filter PostPublished
php artisan nova:filter PostCategories


## creating nova lens
php artisan nova:lens MostTags

## creating nova actions
php artisan nova:action PublishPost
