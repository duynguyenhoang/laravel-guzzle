# Laravel-Guzzle

laravel guzzle service provider

## Install With Composer:

```json
"require": {
    "eleme/laravel-guzzle": "~0.1"
}
```


## Register Service Provider

*/configs/app.php*

```php
    ...
    'providers' => [

        /*
         * Laravel Framework Service Providers...
         */
        ...

        /*
         * Application Service Providers...
         */
        ...
        'Zikaka\Laravel\Providers\Guzzle'
    ],
```


## Enable Facade

*/configs/app.php*

```php
    ...
    'aliases' => [
        ...
        'Guzzle' => 'Zikaka\Laravel\Facades\Guzzle'
    ],
```

## Usage

### Send request

```php

  $response = \Guzzle::get('https://google.com');
```

