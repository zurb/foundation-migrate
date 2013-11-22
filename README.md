foundation-migrate: Migrate to Foundation 5.0+
==================

This plugin will patch Foundation 4 JavaScript initialization code with Foundation 5 syntax and will log a warning that explains the error in your code. Use this plugin to migrate your Foundation 4 JavaScript to Foundation 5 JavaScript.

## How to Use

The first thing to do is to install the Foundation 5 JavaScript, be sure to remove the Foundation 4 libraries:

```html
<script src="js/vendor/jquery.js"></script>
<script src="js/foundation/foundation.min.js"></script>
```

After you have foundation and jQuery included before the closing body tag, drop in the Migrate plugin:

```html
<script src="js/vendor/jquery.js"></script>
<script src="js/foundation/foundation.min.js"></script>
<script src="js/foundation-migrate.js"></script>
```

Then initialize Foundation:

```html
<script src="js/vendor/jquery.js"></script>
<script src="js/foundation/foundation.min.js"></script>
<script src="js/foundation-migrate.js"></script>
<script>
  $(document).foundation();
</script>
```

Once  you are no longer getting any warnings in your console with the *FOUNDATION MIGRATION:* prefix you can remove the `jquery-migrate.js` library from your page.
