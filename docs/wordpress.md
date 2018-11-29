# Wordpress

## Local Dev: Create a new WP site

1. Create DB in XAMPP.
2. [With the `lampp` volume mounted](stack.md?id=mount-lampp-volume), create a new folder for your project in `htdocs` (`/Users/thinktank/.bitnami/YOURUSERNAME/machines/xampp/volumes/root/htdocs`).
3. Download a fresh Wordpress installation from wordpress.org. Put it in the new folder you created.
4. Edit wp-config-sample.php:
- Put in the DB config.
- Copy/paste the security things from the link in the coments.
- Change the filename to remove `sample` so it's just `wp-config.php`.
- add snippet to `wp-config.php` to make custom plugins work.
5. Change the permissions of the site's root directory so you can upload stuff:
`chmod -R 757 foo`

## Local Dev: Pull down existing WP site

## Theming

### Getting your templates to show up

Template hierarchy: https://developer.wordpress.org/themes/basics/template-hierarchy/
