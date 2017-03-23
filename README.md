# Install-WP-TurnkeyLinux-LAMP
Install Wordpress on TurnkeyLinux LAMP via the commandline

```bash
  wget http://wordpress.org/latest.tar.gz
  tar xfz latest.tar.gz
  mv wordpress/* ./
  rmdir ./wordpress/
  rm -f latest.tar.gz
  mysql -u root -p
  create database wordpress;
  create user 'WordpressDBUser'@'localhost' identified by '4qasshole';
  grant usage on *.* to WordpressDBUser@localhost identified by '4qasshole';
  grant all privileges on wordpress.* to WordpressDBUser@localhost;
  use wordpress;
  exit
```

# Install-WP-CLI
Install Wordpress CLI

```bash
  wget https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
  chmod +x wp-cli.phar
  mv wp-cli.phar /usr/local/bin/wp
  wp help
```
