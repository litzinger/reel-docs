---
title: Settings
taxonomy:
    category: docs
---

By default Reel stores it's settings in ExpressionEngine's database, and it is managed via its module settings page. You can also manage it's settings by adding a new array to your site's `config.php` file. You can add as many or as few of the following array keys as you like to the `config.php` file. For example, if you are not using Vimeo, you do not need to add the `settings_vimeo` key and value to the array.

You can't manage some settings in the database, and some settings in the `config.php` file. Either all settings are managed in the `config.php` file, or all settings are managed in the database.

```
$config['reel'] = [
    'settings_global' => [
        'global_width' => '360',
        'global_height' => '240',
    ],
    'settings_youtube' => [
        'user' => '',
        'api_key' => '',
        'show_on_load' => 'n', // 'y' or 'n'
    ],
    'settings_vimeo' => [
        'user' => '',
        'show_on_load' => 'n', // 'y' or 'n'
        'client_id' => '',
        'client_secret' => '',
        'client_token' => '',
    ],
];
```