![image](https://user-images.githubusercontent.com/10347617/156670640-98d1e018-4f21-4293-984b-5ec1a85fbc30.png)


```php
<?php

namespace AndreyHelldar;

use Illuminate\Support\Collection;

class About extends Me
{
    public function getProjects(): Collection
    {
        return collect([
            ['The Dragon Code', 'https://github.com/TheDragonCode'],
            ['Laravel Lang',    'https://github.com/Laravel-Lang'],

            ['Laravel Cashier Provider',  'https://github.com/cashier-provider'],
            ['Laravel Env Sync',          'https://github.com/TheDragonCode/env-sync-laravel'],
            ['Laravel Lang Publisher',    'https://github.com/Laravel-Lang/publisher'],
            ['Laravel Migrate DB',        'https://github.com/TheDragonCode/migrate-db'],
            ['Laravel Migration Actions', 'https://github.com/TheDragonCode/laravel-migration-actions'],
            ['Laravel Pretty Routes',     'https://github.com/TheDragonCode/pretty-routes'],

            ['Package Wizard', 'https://github.com/package-wizard'],
            ['Laraberries',    'https://github.com/Laraberries'],
        ])->mapInto(Project::class);
    }

    /** @return Knowledge[] */
    public function getDailyKnowledge(): array
    {
        return [
            Php::class,
            Laravel::class,
            Docker::class,
            MySQL::class,
            Redis::class,
            ElasticSearch::class,
            RestfulApi::class,
            VueJs::class,
            Git::class,
            Jira::class,
            GitLab::class,
        ];
    }

    public function getProfiles(): array
    {
        return [
            'Website'    => 'https://dragon-code.pro',
            'HabrCareer' => 'https://career.habr.com/helldar',
        ];
    }

    public function getSponsor(): array
    {
        return [
            'https://github.com/sponsors/TheDragonCode',
            'https://www.patreon.com/andrey_helldar',
            'https://yoomoney.ru/to/410012608840929',
        ];
    }
}
```
