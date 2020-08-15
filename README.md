# Laravel 7 API Article Application

Rest API Article Application implemented in Laravel 7.21

#### API's are implemented. 

1. Get All Articles

   GET : http://localhost:8000/api/articles
   
2. Get single Article

   GET : http://localhost:8000/api/articles/50
3. Add new article

   POST : http://localhost:8000/api/articles
4. Update existing Article

   PUT: http://localhost:8000/api/articles/51
5. Delete Article 

   DELETE : http://localhost:8000/api/articles/53  
   
                
####Steps :
1. Copy .env.example file to .env file and update mysql database configuration

2. Run commands :
   
    `composer install`  
    `composer dump-autoload`  
    `composer clear-cache`
   
3. Run command : 
   
   `php artisan serve`
   
   Application will listen on http://127.0.0.1:8000

4. Database Migrations : Migrations script create tables into given database.

   Before actually run migrations script, make sure you have a database created for this app and add its credentials to the .env file located in the root of the project.
   
   `DB_CONNECTION=mysql   
    DB_HOST=127.0.0.1    
    DB_PORT=3306    
    DB_DATABASE=homestead    
    DB_USERNAME=homestead    
    DB_PASSWORD=secret`
 
   Run command : `php artisan migrate` 

5. Database Seeding :
   
   Database seeding is the process of filling up our database with dummy data that we can use to test it.
   
   `php artisan db:seed`

6. Run command : 
   
   `php artisan serve`
   
   Application will listen on http://127.0.0.1:8000   
   
7. Done !!!


   Reference : https://www.toptal.com/laravel/restful-laravel-api-tutorial