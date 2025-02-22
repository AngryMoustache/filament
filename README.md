<p align="center">
    <img src="https://github.com/filamentphp/filament/assets/41773797/8d5a0b12-4643-4b5c-964a-56f0db91b90a" alt="Banner" style="width: 100%; max-width: 800px;" />
</p>

<p align="center">
    <a href="https://github.com/filamentphp/filament/actions"><img alt="Tests passing" src="https://img.shields.io/badge/Tests-passing-green?style=for-the-badge&logo=github"></a>
    <a href="https://laravel.com"><img alt="Laravel v9.x" src="https://img.shields.io/badge/Laravel-v9.x-FF2D20?style=for-the-badge&logo=laravel"></a>
    <a href="https://livewire.laravel.com"><img alt="Livewire v3.x" src="https://img.shields.io/badge/Livewire-v3.x-FB70A9?style=for-the-badge"></a>
    <a href="https://php.net"><img alt="PHP 8.1" src="https://img.shields.io/badge/PHP-8.1-777BB4?style=for-the-badge&logo=php"></a>
</p>

Filament is a collection of full-stack components for accelerated Laravel development. They are beautifully designed, intuitive to use, and fully extensible - the perfect starting point for your next Laravel app. Why waste time building the same features over and over again?

## Packages

### Panel Builder • [Documentation](https://filamentphp.com/docs/panels) • [Demo](https://demo.filamentphp.com)

The panel builder is the foundation of Filament. Combining all the packages together, it allows you to quickly build a Laravel admin panels, customer-facing apps, Software-as-a-Service platforms, and more. Filament makes custom CRUD-driven interfaces feel like a breeze to build and deploy.

```bash
composer require filament/filament
```

### Form Builder • [Documentation](https://filamentphp.com/docs/forms)

Rendering interactive forms in a Livewire component has never been easier than with our form builder. Easily build stunning forms with over 25 components out of the box. It's also fully extensible, so you can add your own custom fields and actions. As well as the panel builder, it is seamlessly integrated into action modals, and is used by the table builder to filter rows.

```bash
composer require filament/forms
```

### Table Builder • [Documentation](https://filamentphp.com/docs/tables)

Craft beautiful, optimized, and interactive datatables for any situation. Drop in to a Livewire component, and you're ready to go. It's also fully extensible, so you can add your own custom columns, filters and actions.

```bash
composer require filament/tables
```

### Notifications • [Documentation](https://filamentphp.com/docs/notifications)

An important part of any application is the ability to notify your users of important events. Our notifications package allows you to deliver flash notifications to users from any Livewire request, or even from your JavaScript frontend. In addition, it can fetch notifications from the database and render them in a beautiful slide-over modal, or even receive live notifications from a websockets server.

```bash
composer require filament/notifications
```

### Actions • [Documentation](https://filamentphp.com/docs/actions)

Actions are buttons that can open modals. They are a very versatile component of many interfaces, avoiding the need for the user to navigate away from the page to complete a task. From confirming a destructive action, to editing an Eloquent record, to importing data from an uploaded CSV file, action modals are a great way to keep the user in the flow of the application. It is built upon our form builder, so it is builds upon the same principles of flexibility and extensibility. Modals can be added to any Livewire component with just a few lines of code, and no HTML or JavaScript.

```bash
composer require filament/actions
```

### Infolists • [Documentation](https://filamentphp.com/docs/infolists)

Infolists are a great way to display read-only information to users about a particular record. They have a fully flexible layout, and can be extended with custom components. They are also seamlessly integrated with the panel builder, so you can easily add them to your panel resources.

```bash
composer require filament/infolists
```

### Widgets • [Documentation](https://filamentphp.com/docs/widgets)

Filament's collection of widgets are built upon Livewire's core principles of real-time reactivity with the server. Combining many widgets allows you to quickly build a dashboard for your application, complete with charts and stats, which are able to update live without refreshing the page. They are also seamlessly integrated with any page in the panel builder.

```bash
composer require filament/widgets
```

## Contributing

If you want to contribute to Filament packages, you may want to test it in a real Laravel project:

- Fork this repository to your GitHub account.
- Create a Laravel app locally.
- Clone your fork in your Laravel app's root directory.
- In the `/filament` directory, create a branch for your fix, e.g. `fix/error-message`.

Install the packages in your app's `composer.json`:

```jsonc
{
    // ...
    "require": {
        "filament/filament": "*",
    },
    "minimum-stability": "dev",
    "repositories": [
        {
            "type": "path",
            "url": "filament/packages/*"
        }
    ],
    // ...
}
```

Now, run `composer update`.

### Checking for missing translations

Set up a Laravel app, and install the [admin panel](https://filamentphp.com/docs/admin/installation).

Now, if you want to check for missing Spanish translations, run:

```bash
php artisan filament:check-translations es
```

This will let you know which translations are missing for this locale. You can make a PR with the changes to this repository.

If you've published the translations into your app and you'd like to check those instead, try:

```bash
php artisan filament:check-translations es --source=app
```

## Need Help?

🐞 If you spot a bug, please [submit a detailed issue](https://github.com/filamentphp/filament/issues/new?assignees=&labels=bug%2Cunconfirmed&template=bug_report.yml), and wait for assistance.

🤔 If you have a question or feature request, please [start a new discussion](https://github.com/filamentphp/filament/discussions/new). We also have a [Discord community](https://filamentphp.com/discord). For quick help, ask questions in the appropriate channel.

🔐 If you discover a vulnerability, please review our [security policy](https://github.com/filamentphp/filament/blob/3.x/SECURITY.md).
