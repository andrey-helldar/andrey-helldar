![won't talk - don't wanna lie](https://user-images.githubusercontent.com/10347617/162590342-4f58279e-1730-4bfe-9ed5-283272770b68.png)

```php
<?php

namespace AndreyHelldar;

class About extends Me
{
    /** @return Collection|Project[] */
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

    public function getContancts(): array
    {
        return [
            'Email'    => 'helldar@dragon-code.pro',
            'Telegram' => 'https://t.me/Helldar'
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
