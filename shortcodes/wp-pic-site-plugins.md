---
slug: wp-pic-site-plugins
title: "wp-pic-site-plugins"
products: [wp-plugin-info-card]
sections: ["shortcodes"]
tags: []
status: publish
---

The `wp-pic-site-plugins` shortcode displays a list of your site's plugins.

<!-- wp:mediaron/alerts-dlx-chakra {"alertType":"warning","alertTitle":"\u003cstrong\u003eThird-party plugins\u003c/strong\u003e","icon":"\u003csvg xmlns=\u0022http://www.w3.org/2000/svg\u0022 height=\u002224\u0022 width=\u002224\u0022 viewBox=\u00220 0 24 24\u0022\u003e\u003cpath d=\u0022M11.983,0a12.206,12.206,0,0,0-8.51,3.653A11.8,11.8,0,0,0,0,12.207,11.779,11.779,0,0,0,11.8,24h.214A12.111,12.111,0,0,0,24,11.791h0A11.766,11.766,0,0,0,11.983,0ZM10.5,16.542a1.476,1.476,0,0,1,1.449-1.53h.027a1.527,1.527,0,0,1,1.523,1.47,1.475,1.475,0,0,1-1.449,1.53h-.027A1.529,1.529,0,0,1,10.5,16.542ZM11,12.5v-6a1,1,0,0,1,2,0v6a1,1,0,1,1-2,0Z\u0022\u003e\u003c/path\u003e\u003c/svg\u003e","uniqueId":"alerts-dlx-bbdef0e4","className":"is-style-warning"} -->
<!-- wp:paragraph {"placeholder":""} -->
<p>Plugins not hosted on the WordPress Plugin Directory are excluded from this site list.</p>
<!-- /wp:paragraph -->
<!-- /wp:mediaron/alerts-dlx-chakra -->

Here's an example of the shortcode in use:

```
[wp-pic-site-plugins cols="2" col_gap="20" row_gap="20" scheme="scheme13" layout="large"]
```

The following are the shortcode parameters.

### id

The ID surrounding the container that contains the site plugins.

### cols

The number of columns (1-3) for the site plugins layout.

### col_gap

The gap between columns in pixels.

### row_gap

The gap between rows in pixels.

### scheme

The scheme used. Can be scheme1 - scheme14.

### layout

The layout used. Can be card, flex, wordpress, ratings, and large.

### {slug}={title} or {slug}="false"

A slug can be set in the shortcode attributes to override the title or disable the plugin from displaying.

Simply use the plugin or theme slug in the shortcode attributes.

Here's an example:

```
[wp-pic-site-plugins cols="2" col_gap="20" row_gap="20" scheme="scheme13" layout="large" easy-digital-downloads="Easy Digital Downloads" query-monitor="false"]
```
