# router

´´´php

require_once("./vendor/Route.php");

use Router\Route;

Route::get("/", function() {
    return "Hello, world";
});

Route::get("/secret", function() {
    return "Hello, secret";
}, function() {
    return true;
});

´´´