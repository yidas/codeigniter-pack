<p align="center">
    <a href="https://codeigniter.com/" target="_blank">
        <img src="https://codeigniter.com/assets/images/ci-logo-big.png" height="100px">
    </a>
    <h1 align="center">CodeIgniter 3 Framework Pack</h1>
    <br>
</p>

Codeigniter 3 complete solution pack with enhanced & modern framework extensions 

[![Latest Stable Version](https://poser.pugx.org/yidas/codeigniter-pack/v/stable?format=flat-square)](https://packagist.org/packages/yidas/codeigniter-pack)
[![License](https://poser.pugx.org/yidas/codeigniter-pack/license?format=flat-square)](https://packagist.org/packages/yidas/codeigniter-pack)

Codeigniter 3 is a great PHP framework with lite portability and high performance, but nowadays it is not so powerful and lacks of design pattern. There are still many maintenance requirements, even suitable development scenario for CodeIgniter 3, so this framework pack provides a total solution to enhance and modernize CodeIgniter 3 with collection of helpful extensions. 

---


OUTLINE
-------

- [Requirements](#requirements)
- [Installation](#installation)
- [Extensions](#extensions)
    - [PSR-4](#psr-4)
    - [ORM Model](#orm-model)
    - [RESTful API](#restful-api)
    - [Widget](#widget)
    - [Unit Test](#unit-test)
    - [Queue Worker](#queue-worker)
- [Configuration](#configuration)
- [Best Practice](#best-practice)
    - [Server Environment](#server-environment)
    - [Application Structure](#application-structure)

---

REQUIREMENTS
------------
This library requires the following:

- PHP 5.4.0+
- CodeIgniter 3.0.0+
- [Extensions Pack](#extensions)

---

INSTALLATION
------------

Run Composer in your CodeIgniter project under the folder `\application`:

    composer require yidas/codeigniter-pack
    
Check CodeIgniter `application/config/config.php`:

```php
$config['composer_autoload'] = TRUE;
```
    
> You could customize the vendor path into `$config['composer_autoload']`

---

EXTENSIONS
----------

### PSR-4
- [yidas/codeigniter-psr4-autoload](https://github.com/yidas/codeigniter-psr4-autoload)  
  *CodeIgniter 3 PSR-4 Autoloader for Application*

### ORM Model
- [yidas/codeigniter-model](https://github.com/yidas/codeigniter-model)  
  *CodeIgniter 3 Active Record (ORM) Standard Model with Laravel Eloquent & Yii2 AR like*

### RESTful API
- [yidas/codeigniter-rest](https://github.com/yidas/codeigniter-rest)  
  *CodeIgniter 3 RESTful API Resource Controller*
  
### Widget
- [yidas/codeigniter-widget](https://github.com/yidas/codeigniter-widget)  
  *CodeIgniter 3 Widget for reusable building view blocks*
  
### Unit Test
- [yidas/codeigniter-phpunit](https://github.com/yidas/codeigniter-phpunit)  
  *CodeIgniter 3 PHPUnit Test extension library*
  
### Queue Worker
- [yidas/codeigniter-queue-worker](https://github.com/yidas/codeigniter-queue-worker)  
  *CodeIgniter 3 Queue Worker Management Controller*

---

CONFIGURATION
-------------

The necessary configurations of the extensions are below:

- [UnitTest Configuration](https://github.com/yidas/codeigniter-phpunit#configuration)

---

BEST PRACTICE
-------------

### Server Environment

[Codeigniter 3 server configuration for Nginx & Apache](https://gist.github.com/yidas/30a611449992b0fac173267951e5f17f)

[Application BaseUrl Setting](https://gist.github.com/yidas/30a611449992b0fac173267951e5f17f#application-baseurl) (Set `/` base for `base_url` at least)

### Application Structure

```
Codeigniter3/
├── application/            CI app root
    ├── cache/              CI cache
    ├── config/             CI app configurations
    ├── contracts           PSR-4 Contracts (ex.Interfaces)
    ├── controllers/        CI app controllers
    ├── core/               CI app level core extension
    ├── helpers/            PSR-4/CI helpers (Recommended to use PSR-4 only)
    ├── hooks/              CI app hooks
    ├── language/           CI app language
    ├── libraries/          CI app components (One time loading)
    ├── logs/               CI app logs
    ├── models/             CI app models (ORM/Active-Record entities)
    ├── presenters/         PSR-4 Presenters
    ├── services/           PSR-4 Services
    ├── third_party/        CI app third party
    ├── vender/             Composer vendor
    ├── views/              CI app views
        └── controller-name/    Each controller has it own view folder
            └── action.php      Each controller action has it own view file
    └── widgets/            PSR-4 Widgets
├── assets/                 Public assets
└── system/                 CI Framework system
```
