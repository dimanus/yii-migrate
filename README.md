yii-migrate
===========

Simple package to add database migrations to project

Installation
------------

* Add to composer.json:

    "require": {
        "grundik/yii-migrate": "*@dev"
    },
    "repositories": [{
      "type": "vcs",
      "url": "https://github.com/Grundik/yii-migrate.git"
    }, {
      "type": "vcs",
      "url": "https://github.com/yiisoft/yii.git"
    }]

* Run composer: composer update

* Create configuration file:
cp vendor/grundik/yii-migrate/config/migrations.php-default config/migrations.php

* Edit configuration file to fulfill your needs: set database credentials, migrations path

* Run
** vendor/bin/migrate - to perform migrate;
** vendor/bin/migrate create <name> - to create new migration.

See also: http://www.yiiframework.com/doc/guide/1.1/en/database.migration