# Drupal Bootcamp

## Installation

### System Requirements

You need to have this installed to configure this project locally:

- [Linux - Ubuntu](https://ubuntu.com/download/desktop)
- [PHP 7.4](https://www.digitalocean.com/community/tutorials/how-to-install-php-7-4-and-set-up-a-local-development-environment-on-ubuntu-20-04)
- [Composer 1](https://getcomposer.org/)
- [Docker](https://www.docker.com/)
- [Lando](https://docs.lando.dev/)

### Local configuration

After install Lando follow these steps:

- Build and start containers in your local environment.
```sh
> lando start
```

You have at your disposal drush to run some commands for Drupal. To run any drush command with this setup you need to:
```sh
> lando drush <command>
```

Here are some lando commands that are useful to you daily:

Start Lando
```sh
> lando start
```

Stop Lando
```sh
> lando stop
```

Restart Lando:
```sh
> lando restart
```

Rebuild Lando (refresh some lando configs, if needed):
```sh
> lando rebuild
```

Destroy Lando (use carefully, because you will loose your database information):
```sh
> lando destroy
```

### Drupal Setup configuration

Information you will need to use with your first Drupal setup for database
```
database: drupal9
username: drupal9
password: drupal9
host: database (doesn't use localhost)
```
