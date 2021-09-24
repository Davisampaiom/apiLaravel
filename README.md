<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel APi
This API is created using Laravel API Resource.

## Installation steps

Follow the bellow steps to install and set up the application.

**Step 1: Clone the Application**<br>
You can download the ZIP file or git clone from my repo into your project  directory.

**Step 2: Configure the Application**<br>
After you clone the repo in to your project folder the project need to be set up by following commands-

- In terminal go to your project directory and Run 
    
        composer install 
    
- Then copy the .env.example file to .env file in the project root folder

- Edit the .env file and fill all required data for the bellow variables
    
        APP_URL=http://localhost //your application domain URL go here
    
        DB_HOST=127.0.0.1 // Your DB host IP. Here we are assumed it to be local host
        DB_PORT=3306 //Port if you are using except the default
        DB_DATABASE=name_of_your_database
        DB_USERNAME=db_user_name
        DB_PASSWORD=db_password
    
- To set the Application key run the bellow command in your terminal.
    
        php artisan key:generate
    
- Make your storage and bootstrapp folder writable by your application user.

- Create all the necessary tables need for the application by runing the bellow command.
    
        php artisan migrate

- Fill default data if your need by running bellow command.

        php artisan db:seed

Thats all! The application is configured now.

### API EndPoints

* Post GET All `http://localhost:8000/api/artigos`
* Post GET Single `http://localhost:8000/api/artigo/{id}`
* Post POST Create `http://localhost:8000/api/novo`
* Post PUT Update `http://localhost:8000/api/atualizar/{id}`
* Post DELETE destroy `http://localhost:8000/api/deleta/{id}`



## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
