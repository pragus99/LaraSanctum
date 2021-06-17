# Laravel REST API with Sanctum

This is an example of a REST API using auth tokens with Laravel Sanctum

## Usage

Change the _.env.example_ to _.env_

```
# Run the webserver
php artisan serve
```

## Routes

```
# Public

GET   /api/products
GET   /api/product/:id

POST   /api/login
@body: email, password

POST   /api/register
@body: name, email, password, password_confirmation


# Protected

POST   /api/product
@body: name, slug, description, price

PUT   /api/product/:id
@body: ?name, ?slug, ?description, ?price

DELETE  /api/product/:id

POST    /api/logout
```
