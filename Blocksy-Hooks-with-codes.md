### Display Shortcode's Content After Blocksy WooCommerce Product Title
```// Display Shortcode's Content After Blocksy WooCommerce Product Title
add_action( 'blocksy:woocommerce:product-card:title:after', 'my_zshcontent', 5 );
function my_zshcontent() {
  print do_shortcode ( '[rwmb_meta id="version" ]' );
}
```
