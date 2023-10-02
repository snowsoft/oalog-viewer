 

## Screenshot

![image](https://user-images.githubusercontent.com/86517067/167827896-7a426d57-ee14-48a3-83e2-eae434d090e0.png)


## Installation

```
$ composer require snowsoft/oalog-viewer

$ php artisan admin:import log-viewer
```

Open `http://localhost/admin/logs`.


## Configuration
If your server doesn't allow you to access log files for example by blocking requests with '.log' in the url you can enable the following bypass function.

See `config/admin.php` and add in the `extensions` section
```php
'extensions' => [
    'log-viewer' => [
        'bypass_protected_urls' => true,
        //'bypass_protected_urls_find' => ['.'],          // default ['.']
        //'bypass_protected_urls_replace' => ['[dot]'],   // default ['[dot]']
    ]
]
```

License
------------
Licensed under [The MIT License (MIT)](LICENSE).
