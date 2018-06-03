<p align="center">
    <a href="https://codeigniter.com/" target="_blank">
        <img src="https://codeigniter.com/assets/images/ci-logo-big.png" height="100px">
    </a>
    <h1 align="center">CodeIgniter 3 Framework Pack</h1>
    <br>
</p>

Codeigniter 3 enhanced & modern framework extensions pack

[![Latest Stable Version](https://poser.pugx.org/yidas/codeigniter-pack/v/stable?format=flat-square)](https://packagist.org/packages/yidas/codeigniter-pack)
[![Latest Unstable Version](https://poser.pugx.org/yidas/codeigniter-pack/v/unstable?format=flat-square)](https://packagist.org/packages/yidas/codeigniter-pack)
[![License](https://poser.pugx.org/yidas/codeigniter-pack/license?format=flat-square)](https://packagist.org/packages/yidas/codeigniter-pack)

Codeigniter 3 is a great PHP framewrok with lite portability and high performance, but nowadays it is not so powerful and lacks of design pattern. There are still many maintenance requirements, even suitable development scenario for Codeigniter 3, so this framework pack provides a total sulotion to enhance and modernize Codeigniter 3 with collection of helpful extensions. 

---

REQUIREMENTS
------------
This library requires the following:

- PHP 5.4.0+
- CodeIgniter 3.0.0+

---

INSTALLATION
------------

Run Composer in your Codeigniter project under the folder `\application`:

    composer require yidas/codeigniter-pack
    
Check Codeigniter `application/config/config.php`:

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
  
### Unit Test
- [yidas/codeigniter-phpunit](https://github.com/yidas/codeigniter-phpunit)  
  *CodeIgniter 3 PHPUnit Test extension library*
