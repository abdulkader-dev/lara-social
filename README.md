# lara-social
laravel social authentication - facebook/twitter/github

### Getting Started

Clone the project repository by running the command below if you use SSH

```
git@github.com:abdulkader-dev/lara-social.git
```

If you use https, use this instead

```
https://github.com/abdulkader-dev/lara-social.git
```

After cloning,run:

```
composer install
```

Duplicate `.env.example` and rename it `.env`

Then run:

```
php artisan key:generate
```

### Migrations And Database Seeder

Be sure to fill in your database details in your `.env` file before running the migrations:

```
php artisan migration
```

### Create an Application

twitter

https://apps.twitter.com/app/new

facebook

https://developers.facebook.com/apps

github

https://github.com/settings/applications/new

visit each link above to create an application  then 

1. Set the callback URL to : { your domain }/auth/twitter/callback 
                          || { your domain }/auth/facebook/callback
                          || { your domain }/auth/github/callback

2. get API Key , API Secret and callback function and add those values on `.env` file.


And finally, start the application:

```
php artisan serve
```

and visit [http://localhost:8000/](http://localhost:8000/) to see the application in action.

