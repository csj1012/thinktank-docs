# Docs!

> Mostly just a place to dump documentation so I don't hate myself later.

## Creating a new (starter) Wordpress Site

1. Create DB in XAMPP.
2. Create folder in .htdocs (lampp -> htdocs)
3. Download a fresh Wordpress installation from wordpress.org. Put it in the new folder you created.
4. Edit wp-config-sample.php:
- Put in the DB config.
- Copy/paste the security things from the link in the coments.
- Change the filename to remove `sample` so it's just `wp-config.php`.
- add snippet to `wp-config.php` to make custom plugins work.
5. Change the permissions of the site's root directory so you can upload stuff:
`chmod -R 757 foo`
