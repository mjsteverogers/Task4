 User List App (Using External API)
This is a Laravel-based web page that displays a list of users fetched from a public API (https://jsonplaceholder.typicode.com/users). It allows you to search users by name — all done directly in the browser using JavaScript.

🔧 What This Project Does
Uses an external API to get user data

Shows a table of user names, emails, and addresses

Lets you search users by name

No need for Laravel controller or database — everything happens in the browser

Files Used
resources/views/users/index.blade.php
This is the only file you need. It contains HTML + CSS + JavaScript to:

Call the API

Display users in a table

Add search and clear features

Show error messages if the API fails

How to Run
Make sure Laravel is installed and working.

Create a route in routes/web.php:

php
Copy
Edit
Route::view('/users', 'users.index');
Create the folder and file:

bash
Copy
Edit
mkdir -p resources/views/users
touch resources/views/users/index.blade.php
Copy the full Blade code (with JavaScript) into that file.

Run Laravel:

bash
Copy
Edit
php artisan serve
Open in browser:
http://127.0.0.1:8000/users

API Used
We are using this public API to get user data:
https://jsonplaceholder.typicode.com/users

This API returns 10 dummy users with their name, email, and address.

Features Demo
Search by name (e.g., try "Leanne")

Clear search button

Error handling if the API doesn't work
