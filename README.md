# router

```php

require_once("./vendor/Route.php");

use Router\Route;

// Ordinary
Route::get("/", function() {
    return "Hello, world";
});

Route::post("/", function() {
    return "Hello, post";
});

Route::put("/", function() {
    return "Hello, put";
});

Route::delete("/", function() {
    return "Hello, delete";
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