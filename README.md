# woocommercehelpbook
WooCommerce help book
- custom hooks and filters to extend/ customize the features of WooCommerce without any plugin
- paste the desired codes in functions.php of your theme/ child theme (before closing tags, if any)

short code for displaying cart (https://github.com/imanishpushkar/woocommercehelpbook/blob/master/show-cart-in-menu): after adding these in functions.php, add the below codes 
as per your need, wherever you want

```php
<?php echo do_shortcode("[woo_cart_but]"); ?>
```

WooCommerce Sidebar (https://github.com/imanishpushkar/woocommercehelpbook/blob/master/woo-sidebar):
after adding these in functions.php, add the below codes in woocommerce.php
 
```php
<?php if (is_active_sidebar('sidebar-woocommerce')) : ?>
  <?php dynamic_sidebar('sidebar-woocommerce'); ?>
<?php else : ?>
  <!-- Time to add some widgets! -->
<?php endif; ?>
```
