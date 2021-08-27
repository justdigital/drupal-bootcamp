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

- Access your local Drupal and follow the installation process
http://local.drupal-bootcamp.com/

If your browser can't open this address, you can try to add this to your hosts, using this command:
```ssh
sudo bash -c 'echo "127.0.0.1 local.drupal-bootcamp.com" >> /etc/hosts'
```

### Drupal Setup configuration

Information you will need to use with your first Drupal setup for database
```
database: drupal9
username: drupal9
password: drupal9
host: database (doesn't use localhost)
```

### Aditional information
You have at your disposal drush to run some commands for Drupal. To run any drush command with this setup you need to:
```sh
> lando drush <command>
```

If you need to access the admin area of Drupal, but doesn't remember your password, you can generate a unique login link using drush:
```sh
> lando drush uli
```

#### Here are some lando commands that are useful to you daily:

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

