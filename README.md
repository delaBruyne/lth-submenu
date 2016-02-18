# lth-submenu

In **Drupal 7**, manage your **secondary tabs menu** as a **block**, for better theming purpose.


## Installation
> drush en lth_submenu -y

## How to use

### Primary level

In `page.tpl.php` :

```php

<?php $primary_tabs = emh_submenu_menu_tabs_primary($tabs);
<?php if (!empty($primary_tabs)): ?>
  <ul class="tabs--primary nav nav-tabs">
    <?php print render($primary_tabs); ?>
  </ul>
<?php endif; ?>
```

### Secondary level

You can now manage your secondary level as a block and show it anywhere in your theme.
