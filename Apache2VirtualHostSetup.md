Navigate to the following directory
```
/etc/apache2/sites-available
```
Create a file in the above directory called `sample.com.conf` 
>Replace all instances of `sample.com` with your domain name

```
<VirtualHost *:80>
  ServerAdmin webmaster@sample.com
  ServerName sample.com
  ServerAlias www.sample.com
  DocumentRoot /var/www/sample.com

  <Directory /var/www/sample.com/>
    Options FollowSymLinks
    AllowOverride All
    Require all granted
  </Directory>

  ErrorLog ${APACHE_LOG_DIR}/sample.com-error.log
  CustomLog ${APACHE_LOG_DIR}/sample.com-access.log combined
</VirtualHost>
```
Open the server (through the shell) and run the following commands
```
ssh root@ipAddress
{enter the password}
```
```
a2ensite sample.com.conf
service apache2 restart
```
---
The site needs to be located in the same directory as `DocumentRoot` from the `conf` file.<br>
The best place to have the sites is in the `/var/www/` directory - one folder per site.
___
Run the following command on the server
```
certbot
```
Now follow through the prompts


