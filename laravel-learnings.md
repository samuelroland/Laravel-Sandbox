# Laravel learnings:

## Starter commands:
### Artisan
- `php artisan serve`: start a server
- `php artisan down`: activate maintenance mode (will return 503 error page in the browser)
- `php artisan up`: disabled maintenance mode

## Project installation

[Installation with composer or the Laravel Installer](https://laravel.com/docs/8.x/installation#installation-via-composer).

```bash
composer create-project laravel/laravel example-app

cd example-app

php artisan serve
```

### Example of directory structure:
```bash

├── README.md
├── app
│   ├── Console
│   │   └── Kernel.php
│   ├── Exceptions
│   │   └── Handler.php
│   ├── Http
│   │   ├── Controllers
│   │   │   ├── Controller.php
│   │   │   └── LoginController.php
│   │   ├── Kernel.php
│   │   └── Middleware
│   │       ├── Authenticate.php
│   │       ├── EncryptCookies.php
│   │       ├── PreventRequestsDuringMaintenance.php
│   │       ├── RedirectIfAuthenticated.php
│   │       ├── TrimStrings.php
│   │       ├── TrustHosts.php
│   │       ├── TrustProxies.php
│   │       └── VerifyCsrfToken.php
│   ├── Models
│   │   ├── Login.php
│   │   └── User.php
│   └── Providers
│       ├── AppServiceProvider.php
│       ├── AuthServiceProvider.php
│       ├── BroadcastServiceProvider.php
│       ├── EventServiceProvider.php
│       └── RouteServiceProvider.php
├── artisan
├── bootstrap
│   ├── app.php
│   └── cache
│       ├── packages.php
│       └── services.php
├── composer.json
├── composer.lock
├── config
│   ├── app.php
│   ├── auth.php
│   ├── broadcasting.php
│   ├── cache.php
│   ├── cors.php
│   ├── database.php
│   ├── filesystems.php
│   ├── hashing.php
│   ├── logging.php
│   ├── mail.php
│   ├── queue.php
│   ├── services.php
│   ├── session.php
│   └── view.php
├── database
│   ├── factories
│   │   └── UserFactory.php
│   ├── migrations
│   │   ├── 2014_10_12_100000_create_password_resets_table.php
│   │   ├── 2019_08_19_000000_create_failed_jobs_table.php
│   │   ├── 2021_02_15_075136_create_companies_table.php
│   │   ├── 2021_02_15_094622_update_users_table.php
│   │   └── users.php
│   └── seeders
│       └── DatabaseSeeder.php
├── package.json
├── phpunit.xml
├── public
│   ├── favicon.ico
│   ├── index.php
│   ├── robots.txt
│   ├── storage
│   └── web.config
├── resources
│   ├── css
│   │   └── app.css
│   ├── js
│   │   ├── app.js
│   │   └── bootstrap.js
│   ├── lang
│   │   └── en
│   │       ├── auth.php
│   │       ├── pagination.php
│   │       ├── passwords.php
│   │       └── validation.php
│   └── views
│       └── welcome.blade.php
├── routes
│   ├── api.php
│   ├── channels.php
│   ├── console.php
│   └── web.php
├── server.php
├── storage
│   ├── app
│   │   └── public
│   ├── framework
│   │   ├── cache
│   │   │   └── data
│   │   │       ├── c0
│   │   │       │   └── 71
│   │   │       │       └── c071422490d526a8aada046adf3a9c9fa0593468
│   │   │       └── ec
│   │   │           └── c4
│   │   │               └── ecc49f49f4da6b940dcde13f0571e79c299871e6
│   │   ├── sessions
│   │   │   ├── 1VtQwg6xACi7Sd0QF3XpfW5E1XbfiG1YCbu1aF8r
│   │   │   └── 9BbEYb8B4Gyur3NFg7W2c2ClpGfBo90yz8fhMwEm
│   │   ├── testing
│   │   └── views
│   │       ├── 21388b61a05d467e0509f6b3ad8bb21d739bca2a.php
│   │       ├── 4e7da541f6cafb4b106b0bcc227d7b37a3a7b7d8.php
│   │       ├── c752a8c5cb9c7b95c562e06881e427703eda5e35.php
│   │       └── f8473e42d19f8c7ee4f0267918b616d67215c6ce.php
│   └── logs
│       └── laravel.log
├── tests
│   ├── CreatesApplication.php
│   ├── Feature
│   │   └── ExampleTest.php
│   ├── TestCase.php
│   └── Unit
│       └── ExampleTest.php
└── webpack.mix.js

```