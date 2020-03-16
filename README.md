# router

```php

require_once("./vendor/Route.php");

use Router\Route;

// Ordinary
Route::get("/", function() {
    return "Hello, world";
});

// Wildcard
Route::get("/wildcard/:id", function() {
    return "Wildcard";
});

// Secret
Route::get("/secret", function() {
    return "Secret";
}, function() {
    return false;
});

```