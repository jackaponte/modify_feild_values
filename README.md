# modify_feild_values

This is a partial port of the VVBO module from Drupal 7 to Backdrop CMS.

It was intended to be the action that allowed an admin to chang any field's value, 
but in my attempt to get it working the scope was decreased as follows:

* instead of workong for all fieldable entities, scope decreased to only node.
* instead of allowing any field to be selected, scope decreased to only a single 
  field with machine name `taxonomy_vocabulary_1`.
* instead of allowing the field to be changed, scope was decreased to removing
  a taxonomy term from the field in question.
* instead of automatically using the field widget, and the settings for its entity, 
  I manually queried the database for possible term ID values and built my own
  select list.
 
 The end result is a module that will allow you to remove a taxonomy term from
 a lot of nodes at a time.
 
 Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules.

- Edit the admin/content view, and check the box for 'Remove category' to enable
  this action.


Current Maintainers
-------------------

- Jen Lampton (https://github.com/jenlampton).

Credits
-------

- Ported to Backdrop CMS by [Jen Lampton](https://www.jenlampton.com).
- Maintained for Drupal by [Graber](https://www.drupal.org/u/graber)
- Maintained for Drupal by [joelpittet](https://www.drupal.org/u/joelpittet)
- Maintained for Drupal by [Jon Pugh](https://www.drupal.org/u/jon-pugh)
- Maintained for Drupal by [bojanz](https://www.drupal.org/u/bojanz)
- Maintained for Drupal by [infojunkie](https://www.drupal.org/u/infojunkie)
- Originally written for Drupal by [Harry Slaughter](https://www.drupal.org/u/harry-slaughter).
- Deveopment Sponsored by [BGP Site Solutions](https://www.bgpsitesolutions.com).

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
