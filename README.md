# PongoCMS v2

### A multilingual CMS built upon Laravel 4 and Bootstrap 3

This package is still under construction... !!  
but you can test it running `composer create-project pongocms/start <your_project_folder>`

#### 1) Add the PongoServiceProvider to app.php

Find your `/app/config/app.php` and add the `PongoServiceProvider`

```php

// app/config/app.php

'providers' => array(
    
    ...

    'Pongo\Cms\PongoServiceProvider',
);
```

#### 2) Create a new Db and set connection data

Create a new database (supported by Laravel) and than set your connection data under `/app/config/database.php` file.

(maybe an automated installer in the future...)

#### 3) Run the Setup command (under construction...)

Open a terminal and run `php artisan pongo:setup`

#### 3) Run a web server and log in

You are almost ready to go!  
Rise your local webserver up with `php artisan serve` and point your browser to `http://localhost:8000/cms`
Your first (admin) account is `admin/admin`.

Happy Pongo!

(...and always remember that this project is in a super-early stage - do not use in production!!)