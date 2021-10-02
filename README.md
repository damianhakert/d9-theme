
# TheMAG - Blog and Magazine Theme for Drupal  
  
TheMAG is a Drupal theme that lets you create a modern magazine website with ease.   
It is ideal for sites that want to rake in ad revenue or profit from content.   
This bestseller theme is perfect for blogging, journalism, or entertainment sites.  
  
TheMAG comes with lots of features and is fully compatible with Drupal Thunder distribution.   
It utilizes and extends the powerful and unique Drupal 8 Layout Builder that lets you create   
complex layouts and pages with few clicks.    
  
## Installation

* Run the Composer to install the core and all dependencies:

```shell script
composer install
```

* Use `drush site:install` to install the site from configuration"

```shell script
vendor/bin/drush site:install \
  --existing-config  \
  --db-url=mysql://DB_USER:DB_PASS@localhost/DB_NAME \
  --account-name="demo" \
  --account-pass="demo" \
  --account-mail="you@example.com"
```

## Demo content

TheMAG comes with two demo content module: 
**TheMAG Default Content** (themag_default_content) and **TheMAG Demo** (themag_demo). 

TheMAG Default Content module has installed by default. 
This module creates some default content to help you start with the theme.

If you'd like to start your site with demo content, then, install the TheMAG demo module (themag_demo). 
TheMAG demo module will create a few nodes, taxonomy terms, blocks, and menu items for demonstration purposes only.

You can install the demo module through the UI or by using Drush:
```shell script
drush en -y themag_demo
```

In the end, you can uninstall both the demo and the default content module as well as their required modules. 
Uninstalling demo modules won't remove the created content. Instead, you'll need to do that manually.

## Updating core and modules

To update the core and the modules at the same time, run:
```shell script
composer update --with-dependencies
```

To update only the core, run:
```shell script 
composer update drupal/core-recommended --with-dependencies
```

When the composer finish, run `drush updatedb` or `update.php`.

## TheMAG documentation

For more extensive documentation on how to use TheMAG please visit the documentation page at: 
[https://docs.themag.pinkdexo.com](https://docs.themag.pinkdexo.com)
