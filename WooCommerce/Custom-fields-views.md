### Replace Short Description with Shortcode's content
```
// Replace Short Description with Shortcode's content
add_filter('woocommerce_short_description', function ($description) {
	if (! is_product()) { return; }   
	return do_shortcode('[mbv name="product-info"]');
});
```
### Display Shortcode's Content After WooCommerce short Description

```
// Display Shortcode's Content After WooCommerce short Description 
add_filter('woocommerce_short_description', function ($description) {
	if (! is_product()) { return; }   
	return $description.do_shortcode('[mbv name="product-info"]');
});
```
