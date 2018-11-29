### If a client needs hosting
Recommend to clients:
- HostGator or GoDaddy or similar

# To Launch

Someone will (on the client side, but you may have to):

- sign up for hosting
- point the DNS to the hosting

## HostGator

### Existing WordPress Site via HostGator WordPress package

1. Go to Hosting > Manage package

1. On your local machine, set hosts file entry to the new site IP from the host `sudo nano /etc/hosts`. This is so you can run the installer at `wp-installer.php` on the destination (live) site.

1. Create a FTP account on the hosting account site. Add the account username/password/etc. to the `logins` file on the ThinkTank Clients server for that project.

1. Use your FTP client (or CPanel) to upload the site files to the host in `/`

1. Download `wp-config.php` from the existing codebase and open it to get the Database settings (if they have an exisiting blank WP install through purchasing a WordPress package, otherwise you can use PHPMyAdmin or some other way to get to the database).

1. Get rid of the existing codebase.

1. Using Duplicator (admin > Duplicator), export the staging site and files. Click the Installer and Archive buttons, or use One-Click Download.

1. Paste the downloaded files from Duplicator in the live site directory.

1. Go through the Duplicator prompt at `/install.php`.

1. Tell whoever's pointing the DNS to point the DNS after you've checked out the site and it looks good.

1. Turn on the "Really Simple SSL plugin"

1. Let Trish and Kevin know that the site is uploaded.
