# wp-project

This is a lightweight composer package for quickly installing the
files needed for a clean, decoupled WordPress.

WordPress files and working content directories are separated, making
version control cleaner.

```
git clone git@github.com:Sideways8/wp-project.git ./your-project-name

cd your-project-name && composer install
```

This will:
- Download WordPress to /www/wp
- Create content directories in /www/content (plugins, )
- Create multi-environment configuration files in /config
- Download a fresh set of auth salts from WordPress

Edit **/config/wp-config-dev.php**:
- Set the APP_DOMAIN to your instance's domain (ie, mysite.wp)
- Set the DB_ constants to connect to your database.

Finally, serve the /www directory from your web server.