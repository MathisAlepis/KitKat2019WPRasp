# KitKat2019WPRasp

Win32DiskImager : [lien](https://sourceforge.net/projects/win32diskimager/).
Raspbian : [lien](https://www.raspberrypi.org/downloads/raspbian/).

## Installation

```bash
$ sudo apt-get update upgrade
$ sudo apt-get install -y nginx php php-fpm mysql-server php-mysql
$ sudo mysql --user=root
DROP USER 'root'@'localhost';
CREATE USER 'root'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON *.* TO 'root'@'localhost';
$ sudo mysql -u root -ppassword
create database wordpress;
$ cd /var/www/html
$ sudo tar xzf latest.tar.gz
$ sudo chown -R www-data /var/www/html/wordpress
$ sudo wget https://raw.githubusercontent.com/MathisAlepis/KytCat2019WPRasp/master/wordpress
$ sudo ln -s /etc/nginx/sites-available/<nom_de_votre_site> /etc/nginx/sites-enabled/<nom_de_votre_site>
$ sudo /etc/init.d/nginx restart
```

IP interne :

```bash
$ ifconfig
```

IP Publique : [lien](https://www.monippublique.com/).

Pour les autres FAI : [lien](https://www.it-connect.fr/rendre-son-serveur-web-accessible-depuis-internet/)
