![won't talk - don't wanna lie](https://user-images.githubusercontent.com/10347617/163692044-d059e2f8-0137-427b-a5e4-7f6864167e9a.png)


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

            ['Laravel Migration Actions', 'https://github.com/TheDragonCode/laravel-migration-actions'],
            ['Laravel Cashier Provider',  'https://github.com/cashier-provider'],
            ['Laravel Pretty Routes',     'https://github.com/TheDragonCode/pretty-routes'],
            ['Laravel Lang Publisher',    'https://github.com/Laravel-Lang/publisher'],
            ['Laravel Migrate DB',        'https://github.com/TheDragonCode/migrate-db'],
            ['Laravel Env Sync',          'https://github.com/TheDragonCode/env-sync-laravel'],

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
            'LinkedIn'   => 'https://www.linkedin.com/in/helldar',
        ];
    }

    public function getContacts(): array
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
            'https://yoomoney.ru/to/410012608840929',
        ];
    }
}
```
