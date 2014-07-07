[![Latest Stable Version](https://poser.pugx.org/pongocms/start/v/stable.svg)](https://packagist.org/packages/pongocms/start) [![Total Downloads](https://poser.pugx.org/pongocms/start/downloads.svg)](https://packagist.org/packages/pongocms/start) [![Latest Unstable Version](https://poser.pugx.org/pongocms/start/v/unstable.svg)](https://packagist.org/packages/pongocms/start) [![License](https://poser.pugx.org/pongocms/start/license.svg)](https://packagist.org/packages/pongocms/start)

# PongoCMS v2

### A multilingual CMS built upon Laravel 4 and Bootstrap 3

This package is still under construction... !!  
but you can test it running `composer create-project pongocms/start <your_project_folder>`

#### 1) Add Service Providers to app.php

Find your `/app/config/app.php` and add to the `providers` section both the `PongoServiceProvider` and the `SiteServiceProvider`

```php

// app/config/app.php

'providers' => array(
    
    ...

    'Pongo\Cms\PongoServiceProvider',
    'Pongo\Site\SiteServiceProvider',
);
```

#### 2) Create a new Db and set connection data

Create a new database (supported by Laravel) and than set your connection data under `/app/config/database.php` file.

(maybe an automated installer in the future...)

#### 3) Run the Setup command

Open a terminal and run `php artisan pongo:setup`

#### 4) Run a web server and log in

You are almost ready to go!  
Rise your local webserver up with `php artisan serve` and point your browser to `http://localhost:8000/cms`
Your first (admin) account is `admin/admin`.

Happy Pongo!

(...and always remember that this project is in a super-early stage - do not use in production!!)
