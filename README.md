My laravel Nova package studies

# Commands used

## Laravel instalation
sudo chmod 0777 -R storage/
php artisan key:generate
composer require laravel/scout
php artisan vendor:publish --provider="Laravel\Scout\ScoutServiceProvider"
composer require algolia/algoliasearch-client-php

## Instaling Nova
php artisan Nova:install

## creating a user
php artisan Nova:user

## migrations
php artisan make:migration create_posts_table
php artisan make:migration --table=posts add_more_post_columns
php artisan make:migration create_post_tag_table

## making the laravel models
php artisan make:model Post
php artisan make:model Tag


## making the Nova resources
php artisan Nova:resource Post
php artisan Nova:resource Tag


## creating laravel policies
php artisan make:policy PostPolicy -m Post

## creating Nova filters
php artisan Nova:filter PostPublished
php artisan Nova:filter PostCategories


## creating Nova lens
php artisan Nova:lens MostTags

## creating Nova actions
php artisan Nova:action PublishPost

## creating Nova metrics
php artisan nova:value PostCount