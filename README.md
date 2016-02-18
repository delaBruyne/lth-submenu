# lth-submenu

In **Drupal 7**, manage your **secondary tabs menu** as a **block**, for better theming purpose.


## Installation
Download this module in your `/modules` directory :
> git clone git@github.com:delaBruyne/lth_submenu.git

Then activate it throught Drupal BO or with drush :
> drush en lth_submenu -y

## How to use

### Primary level

In `page.tpl.php` :

```php

<?php $primary_tabs = lth_submenu_menu_tabs_primary($tabs);
<?php if (!empty($primary_tabs)): ?>
  <ul class="tabs--primary">
    <?php print render($primary_tabs); ?>
  </ul>
<?php endif; ?>
```

### Secondary level

You can now manage your secondary level as a block and show it anywhere in your theme.
