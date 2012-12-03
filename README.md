# MongoDB User managemant for [Lithium PHP framework](http://lithify.me/)

Inspired by li3_usermanager li3_mongouman's goal is to provide the same functionality but built with MongoDB in mind.

* User registration
* User activation trough link with token
* Password resets trough link with token
* Updating user data (email, password, about...)
* Log in / log out
* Access control trough AccessController (user auth data inspection)
* User managemant (allowed for admins/root)
  * Promotion (group change)
  * Activation / deactivation
  * Editing users (email, password, about...)
* Session Control via MongoDB

## Instalation - Warning: Proejct Pre-Alpha Do not Use Yet

Checkout **li3_mongouman** to either of your library directories:

	cd libraries
	git clone git://github.com/fitzagard/li3_mongouman.git

Then load it in your main app config. Open `app/config/bootstrap/libraries.php` with your favorite
editor, and add:

	Libraries::add('li3_mongouman');

Setup `default` MongoDB database connection in your `app/config/bootstrap/connections.php`.
Uncoment `require` for `connections.php` and `session.php` in your `app/config/bootstrap.php`

### Install Submodule Dependencies

Clone dependencies to your `libraries` and load them in `app/config/bootstrap/libraries.php`.

This plugins use:

* li3_mailer
* swiftmailer
* li3_access

## TODO

* Build the entire project :)

Status: Unstable