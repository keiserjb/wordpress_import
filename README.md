Wordpress Import
================

This Drupal module imports a WordPress blog from a WordPress eXtended RSS (WXR)
format file.


Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

- Visit the page under Administration > Content > Wordpress Import
  and follow the steps.

Documentation
-------------

Additional documentation is located in the Wiki: https://github.com/bjoern-st/wordpress_import/wiki/Documentation

Issues
------

 - No rollback if something wrong happens. You must make a backup of your
   database before importing a blog. You can use an extra module such as "Backup
   and Migrate" to easily backup your Drupal database.

 - User passwords aren't transferred from WordPress, a password for new users
   must be set after importing. This is a limitation of the WordPress WXR export
   format.

 - Blogroll isn't imported because it isn't included in the WXR export file
   created by WordPress. However, you can find instructions on how to export
   your site's blogroll as an OPML file : http://codex.wordpress.org/FAQ_Working_with_WordPress#How_do_I_import_links_.28blogroll.29_from_another_WordPress_blog.3F

   This OPML file can then be imported into Drupal through a module such as
   Feeds : http://drupal.org/project/feeds

 - Special WordPress tags such as [video] and [caption] are not automatically
   translated into HTML

 - Password-protected posts are imported as unpublished nodes. This function can
   be replicated using this module : http://drupal.org/project/protected_node

 - WordPress redirects, attachments and custom fields are not imported, patches
   welcome.

Current Maintainers
-------------------

- Bjoern (https://github.com/bjoern-st)

Credits
-------

Originally written for Drupal by Jerome Charaoui, aka lavamind (http://www.koumbit.org/)
Originally written for Drupal by Yann Rocq (http://www.rocq.net/yann/)

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
