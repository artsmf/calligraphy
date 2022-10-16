
### Custom CSS
To implement custom CSS sitewide, change the config.toml parameter `customCSS` from `false` to `true` and then create a `css.html` file in your `layouts/partials/` folder like the example below:

```html
<style>
  <!-- This will remove the shadow on the navbar -->
  nav {
    box-shadow: none;
  }
</style>
```

This will render inline CSS in the head of your site and without adding an extra HTTP request.

### Cache Busting
As of `v2.1.0`, this theme uses native [Hugo Pipes](https://gohugo.io/hugo-pipes/introduction/) for cache busting of assets. Generated assets will be served from the `resources` folder and will no longer require any additional setup with Gulp.

## License
This theme is released under the Apache 2.0 license. For more information read the [license](https://github.com/tomanistor/osprey/blob/master/LICENSE).
