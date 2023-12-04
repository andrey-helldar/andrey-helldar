![Untitled-1](https://github.com/andrey-helldar/andrey-helldar/assets/10347617/a8cb924d-eb2a-4ce9-8925-469acd74a090)

```php
<?php

namespace AndreyHelldar;

/*
 * Always write code like it’s going to be supported by an unstable,
 * violent psychopath who knows where you live.
 */
class About extends Me
{
    /** @return Collection<Organization> */
    public function getOrganizations(): Collection
    {
        return collect([
            ['The Dragon Code',     'https://github.com/TheDragonCode'],
            ['Laravel Lang',        'https://github.com/Laravel-Lang'],
            ['Cashbox for Laravel', 'https://github.com/cashbox-laravel'],
            ['Volunteers CRM',      'https://github.com/volunteers-crm'],
            ['Package Wizard',      'https://github.com/package-wizard'],
            ['Laraberries',         'https://github.com/Laraberries'],
        ])->mapInto(Organization::class);
    }

    /** @return Collection<Project> */
    public function getTheBestProjects(): Collection
    {
        return collect([
            ['Actions',                'https://github.com/TheDragonCode/laravel-actions'],
            ['Migrate DB',             'https://github.com/TheDragonCode/migrate-db'],
            ['Laravel Lang Publisher', 'https://github.com/Laravel-Lang/publisher'],
            ['Cashbox for Laravel',    'https://github.com/cashbox-laravel'],
            ['Pretty Routes',          'https://github.com/TheDragonCode/pretty-routes'],
            ['Env Sync',               'https://github.com/TheDragonCode/env-sync-laravel'],
            ['HTTP Logger',            'https://github.com/TheDragonCode/laravel-http-logger'],
            ['JSON Response',          'https://github.com/TheDragonCode/laravel-json-response'],
            ['Laravel Cache',          'https://github.com/TheDragonCode/laravel-cache'],
            ['Simple DTO',             'https://github.com/TheDragonCode/simple-data-transfer-object'],
            ['Which Color',            'https://github.com/TheDragonCode/which-color'],
        ])->mapInto(Project::class);
    }

    /** @return array<string> */
    public function getDailyKnowledge(): array
    {
        return [
            'laravel', 'php', 'docker', 'mysql', 'redis',
            'elasticsearch', 'vuejs', 'git', 'jira', 'gitlab'
        ];
    }

    /** @return Collection<Profile> */
    public function getProfiles(): Collection
    {
        return collect([
            'Website'    => 'https://dragon-code.pro',
            'HabrCareer' => 'https://career.habr.com/helldar',
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

    /** @return array<string> */
    public function getSponsor(): array
    {
        return [
            'https://github.com/sponsors/TheDragonCode',
            'https://yoomoney.ru/to/410012608840929',
            'https://boosty.to/dragon-code',
            'https://www.donationalerts.com/r/dragon_code',
        ];
    }
}
```

![3d profile](./profile-3d-contrib/profile-south-season-animate.svg)
