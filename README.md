# <center>Laravel Coding Standard Structure</center>

## Table of Contents
-----------------

* [<b>Introduction</b>](#introduction)
* [Project Structure](#project-structure)
* [Controllers](#controllers)
* [Models](#models)
* [Views](#views)
* [Routes](#routes)
* [Middleware](#middleware)
* [Services](#services)
* [Events](#events)
* [Listeners](#listeners)
* [Jobs](#jobs)
* [Commands](#commands)
* [API Documentation](#api-documentation)
* [Naming Naming Conventions](#naming-convention)

## Introduction
------------

This is a Laravel project that provides a basic **Coding Flow**.

## Project Structure
------------------

The project is structured as follows:
###### App
* `app/`: The application directory.
###### Requests
* `app/Http/Requests/Backend`: The requests directory for BE.
* `app/Http/Requests/Frontend`: The requests directory for FE.
###### Rules
* `app/Rules/Backend`: The rules directory for BE.
* `app/Rules/Frontend`: The rules directory for FE.
###### Traits
* `app/Traits/Backend`: The traits directory for BE.
* `app/Traits/Frontend`: The traits directory for FE.
###### Helpers
* `app/Helpers/Backend`: The helpers directory for BE.
* `app/Helpers/Frontend`: The helpers directory for FE.
###### Controllers
* `app/Http/Controllers/Backend`: The controllers directory for BE.
* `app/Http/Controllers/Frontend`: The controllers directory for FE.
###### Models
* `app/Models/`: The models directory.
###### Views
* `resources/views/`: The views directory.
* `resources/views/backend`: The views directory for BE.
* `resources/views/frontend`: The views directory for FE.

###### Routes
* `routes/`: The routes directory.
* `routes/backend.php`: The BE routes file.
* `routes/frontend.php`: The FE routes file.
* `routes/api.php`: The API routes file.
* `routes/web.php`: The web routes file.

## Controllers
-------------

### UserController

* `index()`: Returns a list of all users.
* `show($id)`: Returns a single user by ID.
* `store(Request $request)`: Creates a new user.
* `update(Request $request, $id)`: Updates an existing user.
* `destroy($id)`: Deletes a user.

### Example Usage

<details>
  <summary>Title 1</summary>
  Content related to Title 1
</details>

<details>
  <summary>Title 2</summary>
  Content related to Title 2
</details>

### Example Usage

```php
// Create a new user
$user = new User();
$user->name = 'John Doe';
$user->email = 'john@example.com';
$user->save();

// Update an existing user
$user = User::find(1);
$user->name = 'John Smith';
$user->save();
