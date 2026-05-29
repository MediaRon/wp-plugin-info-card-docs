---
description: Display a list of all of your site's plugins
---

# wp-pic-site-plugins

The `wp-pic-site-plugins` shortcode displays a list of your site's plugins.

{% hint style="danger" %}
**Third-party plugins:** (plugins not hosted on the WordPress Plugin Directory) are excluded from this site list.
{% endhint %}

Here's an example of the shortcode in use:

{% code overflow="wrap" %}
```
[wp-pic-site-plugins cols="2" col_gap="20" row_gap="20" scheme="scheme13" layout="large"]
```
{% endcode %}

The following are the shortcode parameters.

### id

The ID surrounding the container that contains the site plugins.

### cols

The number of columns (1-3) for the site plugins layout.

### col\_gap

The gap between columns in pixels.

### row\_gap

The gap between rows in pixels.

### scheme

The scheme used. Can be scheme1 - scheme14.

### layout

The layout used. Can be card, flex, wordpress, ratings, and large.

### {slug}={title} or {slug}="false"

A slug can be set in the shortcode attributes to override the title or disable the plugin from displaying.

Simply use the plugin or theme slug in the shortcode attributes.

Here's an example:

{% code overflow="wrap" %}
```
[wp-pic-site-plugins cols="2" col_gap="20" row_gap="20" scheme="scheme13" layout="large" easy-digital-downloads="Easy Digital Downloads" query-monitor="false"]
```
{% endcode %}
