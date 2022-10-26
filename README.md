![peace](https://user-images.githubusercontent.com/10347617/183268386-c25ec9ae-6af9-4855-97fb-7ef29f54015d.png)

```php
<?php

namespace AndreyHelldar;

class About extends Me
{
    /** @return Collection<Organization> */
    public function getOrganizations(): Collection
    {
        return collect([
            ['The Dragon Code',           'https://github.com/TheDragonCode'],
            ['Laravel Lang',              'https://github.com/Laravel-Lang'],
            ['Volunteers CRM',            'https://github.com/volunteers-crm'],
            ['Laravel Cashier Provider',  'https://github.com/cashier-provider'],
            ['Package Wizard',            'https://github.com/package-wizard'],
            ['Laraberries',               'https://github.com/Laraberries'],
        ])->mapInto(Organization::class);
    }

    /** @return Collection<Project> */
    public function getTheBestProjects(): Collection
    {
        return collect([
            ['Laravel Migration Actions', 'https://github.com/TheDragonCode/laravel-migration-actions'],
            ['Laravel Migrate DB',        'https://github.com/TheDragonCode/migrate-db'],
            ['Laravel Lang Publisher',    'https://github.com/Laravel-Lang/publisher'],
            ['Laravel Pretty Routes',     'https://github.com/TheDragonCode/pretty-routes'],
            ['Laravel Env Sync',          'https://github.com/TheDragonCode/env-sync-laravel'],
            ['Laravel Cashier Provider',  'https://github.com/cashier-provider'],
            ['Laravel HTTP Logger',       'https://github.com/TheDragonCode/laravel-http-logger'],
            ['Laravel JSON Response',     'https://github.com/TheDragonCode/laravel-json-response'],
            ['Laravel Cache',             'https://github.com/TheDragonCode/laravel-cache'],
            ['Simple DTO',                'https://github.com/TheDragonCode/simple-data-transfer-object'],
            ['Which Color',               'https://github.com/TheDragonCode/which-color'],
            // ...
        ])->mapInto(Project::class);
    }

    public function getDailyKnowledge(): array
    {
        return [
            Laravel::class,
            Php::class,
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

    /** @return Collection<Profile> */
    public function getProfiles(): Collection
    {
        return collect([
            'Website'    => 'https://dragon-code.pro',
            'HabrCareer' => 'https://career.habr.com/helldar',
            'LinkedIn'   => 'https://www.linkedin.com/in/helldar',
        ])->mapInto(Profile::class);
    }

    /** @return Collection<Contact> */
    public function getContacts(): array
    {
        return collect([
            'Email'    => 'helldar@dragon-code.pro',
            'Telegram' => 'https://t.me/Helldar',
        ])->mapInto(Contact::class);
    }

    public function getSponsor(): array
    {
        return [
            'https://github.com/sponsors/TheDragonCode',
            'https://yoomoney.ru/to/410012608840929',
            'https://boosty.to/dragon-code',
        ];
    }
}
```

![3d profile](./profile-3d-contrib/profile-south-season-animate.svg)
