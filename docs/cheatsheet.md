# Josh's Cheatsheet

> Josh's cheatsheet of miscellaneous stuff that I'm dumping here before he leaves :( 

## Change where a site points

`sudo nano /etc/hosts`

## Change permissions to a WordPress site

`chmod -R 757 /Applications/XAMPP/xamppfiles/htdocs/withchangeinmind-org`

## Set up Stage Site

1. `ssh root@192.168.0.253`

2. Enter the password. You know the one.

3. `nano /etc/httpd/conf/httpd.conf`

In httpd.conf:

```
<VirtualHost *:80>
ServerName project-name.thinktankprm.com
ServerAlias project-name.thinktankprm.com
DocumentRoot /var/www/html/project-name
ErrorLog /var/www/html/project-name/error.log
CustomLog /var/www/html/project-name/request.log combined
</VirtualHost>
```

`sudo chown apache:apache /var/www/html/project-name`

`sudo httpd -k restart`

## Local MySQL Start

`sudo /Applications/XAMPP/xamppfiles/bin/mysql.server start`
