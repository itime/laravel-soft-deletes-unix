# Laravel SoftDeletes With Unix Timestamp
### forked from [al-one/laravel-soft-deletes-unix](https://github.com/al-one/laravel-soft-deletes-unix)

## Installing

```sh
$ composer require itime/laravel-soft-deletes-unix -vvv
```

or 

```sh
$ composer require itime/laravel-soft-deletes-unix:dev-master -vvv
```


## Usage

```php
<?php

namespace App;

use Illuminate\Database\Eloquent\Model;
use Itime\LaravelSoftDeletesUnix\Eloquent\SoftDeletesUnix;

class Flight extends Model
{

    use SoftDeletesUnix;

    protected $dateFormat = 'U';

    protected $dates = ['deleted_at'];
}
```

## License

MIT