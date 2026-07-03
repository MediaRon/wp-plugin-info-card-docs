---
slug: wp-pic
title: "wp-pic"
products: [wp-plugin-info-card]
sections: ["shortcodes"]
tags: []
status: publish
---

The `wp-pic` shortcode can be used to display a single or multiple plugins. See below for the shortcode parameters.

Example shortcode:

```
[wp-pic slug="simple-revisions-delete" layout="large" scheme="scheme1" align="right" margin="0 0 0 20px" containerid="download-sexion" ajax="yes"]// Some code
```

### type

Can be of type `plugin` or `theme`. Type `plugin` is default.

```
[wp-pic type="theme" slug="zerif-lite"]
```

### slug

The `slug` (required) parameter can be a single or comma-separated string of plugin slugs.

```
[wp-pic slug="wp-plugin-info-card"]
```

Comma-separate the slugs to be in **multi** mode, which will output multiple plugins.

```
[wp-pic slug="highlight-and-share,simple-comment-editing" multi="true" cols="2" col_gap="40" row_gap="40"]
```

### {slug}={title}

A slug can be set in the shortcode attributes to override the title.

Simply use the plugin or theme slug in the shortcode attributes.

<!-- wp:dlxplugins/photo-block {"uniqueId":"photo-block-e85d5ac4","date":1780285151123,"globalStyle":"dlxkb-image","imageData":{"id":42500,"url":"https://docs.dlxplugins.com/wp-content/uploads/2026/05/dlx-2024Jl6Uiy21402x-1024x576.jpg","alt":"Plugin Info Cards With Custom Titles","full":"https://docs.dlxplugins.com/wp-content/uploads/2026/05/dlx-2024Jl6Uiy21402x.jpg","width":1024,"height":576,"title":"","caption":"","attachment_link":"https://docs.dlxplugins.com/product/wp-plugin-info-card/wp-pic/screenshot-42/","file_size":"38.4 KB","dimensions":{"width":1024,"height":576},"edit_nonce":"44f290589b","crop_nonce":"12c85bf4a0","can_edit":true},"photoDropShadow":{"color":"#3F3F37","opacity":0.85,"blur":10,"spread":2,"horizontal":2,"vertical":2,"inset":false,"enabled":true},"containerWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"","unit":""}},"containerMaxWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"800","unit":"px"}},"photoMode":"photo","mediaLinkType":"image","mediaLinkOverride":true,"hasCaption":true,"lightboxEnabled":true} -->
<!-- wp:dlxplugins/photo-caption-block {"globalStyle":"dlxkb-image","uniqueId":"photo-block-e85d5ac4","captionManual":"Plugin Info Cards With Custom Titles","captionTypography":{"mobile":{"fontFamily":"","fontFamilySlug":"","fontSize":"","fontSizeUnit":"px","fontWeight":"","lineHeight":"","lineHeightUnit":"em","textTransform":"","letterSpacing":"","letterSpacingUnit":"px","fontFallback":"","fontType":"web"},"tablet":{"fontFamily":"","fontFamilySlug":"","fontSize":"","fontSizeUnit":"px","fontWeight":"","lineHeight":"","lineHeightUnit":"em","textTransform":"","letterSpacing":"","letterSpacingUnit":"px","fontFallback":"","fontType":"web"},"desktop":{"fontFamily":"Verdana, sans-serif","fontFamilySlug":"verdana","fontSize":"18","fontSizeUnit":"px","fontWeight":"normal","lineHeight":"1.2","lineHeightUnit":"em","textTransform":"none","letterSpacing":"0","letterSpacingUnit":"px","fontType":"web","fontFallback":"sans-serif"}},"captionMarginSize":{"mobile":{"top":"","right":"","bottom":"","left":"","topUnit":null,"rightUnit":null,"bottomUnit":null,"leftUnit":null,"unitSync":true},"tablet":{"top":"","right":"","bottom":"","left":"","topUnit":null,"rightUnit":null,"bottomUnit":null,"leftUnit":null,"unitSync":true},"desktop":{"top":"8","right":"0","bottom":"0","left":"0","topUnit":"px","rightUnit":"px","bottomUnit":"px","leftUnit":"px","unitSync":false}},"containerWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"","unit":""}}} /-->
<!-- /wp:dlxplugins/photo-block -->

Here's an example:

```
[wp-pic slug="wp-plugin-info-card,highlight-and-share" multi="true" cols="2" highlight-and-share="test highlight" wp-plugin-info-card="test"]
```

You can do the same for themes:

<!-- wp:dlxplugins/photo-block {"uniqueId":"photo-block-9ae58277","globalStyle":"dlxkb-image","imageData":{"id":42501,"url":"https://docs.dlxplugins.com/wp-content/uploads/2026/05/dlx-2024RrHMTUev402x-1024x576.jpg","alt":"Theme Custom Titles","full":"https://docs.dlxplugins.com/wp-content/uploads/2026/05/dlx-2024RrHMTUev402x.jpg","width":1024,"height":576,"title":"","caption":"","attachment_link":"https://docs.dlxplugins.com/product/wp-plugin-info-card/wp-pic/screenshot-43/","file_size":"44.3 KB","dimensions":{"width":1024,"height":576},"edit_nonce":"d854d743b3","crop_nonce":"63e82f1758","can_edit":true},"photoDropShadow":{"color":"#3F3F37","opacity":0.85,"blur":10,"spread":2,"horizontal":2,"vertical":2,"inset":false,"enabled":true},"containerWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"","unit":""}},"containerMaxWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"800","unit":"px"}},"photoMode":"photo","mediaLinkType":"image","hasCaption":true,"lightboxEnabled":true} -->
<!-- wp:dlxplugins/photo-caption-block {"globalStyle":"dlxkb-image","uniqueId":"photo-block-9ae58277","captionManual":"Theme Custom Titles","captionTypography":{"mobile":{"fontFamily":"","fontFamilySlug":"","fontSize":"","fontSizeUnit":"px","fontWeight":"","lineHeight":"","lineHeightUnit":"em","textTransform":"","letterSpacing":"","letterSpacingUnit":"px","fontFallback":"","fontType":"web"},"tablet":{"fontFamily":"","fontFamilySlug":"","fontSize":"","fontSizeUnit":"px","fontWeight":"","lineHeight":"","lineHeightUnit":"em","textTransform":"","letterSpacing":"","letterSpacingUnit":"px","fontFallback":"","fontType":"web"},"desktop":{"fontFamily":"Verdana, sans-serif","fontFamilySlug":"verdana","fontSize":"18","fontSizeUnit":"px","fontWeight":"normal","lineHeight":"1.2","lineHeightUnit":"em","textTransform":"none","letterSpacing":"0","letterSpacingUnit":"px","fontType":"web","fontFallback":"sans-serif"}},"captionMarginSize":{"mobile":{"top":"","right":"","bottom":"","left":"","topUnit":null,"rightUnit":null,"bottomUnit":null,"leftUnit":null,"unitSync":true},"tablet":{"top":"","right":"","bottom":"","left":"","topUnit":null,"rightUnit":null,"bottomUnit":null,"leftUnit":null,"unitSync":true},"desktop":{"top":"8","right":"0","bottom":"0","left":"0","topUnit":"px","rightUnit":"px","bottomUnit":"px","leftUnit":"px","unitSync":false}},"containerWidth":{"mobile":{"width":"","unit":null},"tablet":{"width":"","unit":null},"desktop":{"width":"","unit":""}}} /-->
<!-- /wp:dlxplugins/photo-block -->

```
[wp-pic type="theme" slug="twentytwentyfour,twentytwentythree" multi="true" cols="2" twentytwentyfour="2024" twentytwentythree="2023"]
```

### marginSpacing

This can be set to improve the margin around the plugin card.

- none
- compact
- comfortable
- spacious
- extreme

### marginTarget

Used to target the top, bottom, or both margins of the plugin card.

- both
- top
- bottom

### multi

This must be set to `true` if there are multiple slugs. The following extra attributes assist in `multi` output:

- **cols** (1-3)
- **col_gap** - Gap in pixels between items
- **row_gap** - Gap in pixels between rows

```
[wp-pic slug="highlight-and-share,simple-comment-editing" multi="true" cols="2" col_gap="40" row_gap="40"]
```

### layout

Default is “card” so you may leave this parameter empty. The default layout can be set in the admin settings.

Available layouts are:

- card
- large
- flex
- wordpress
- ratings

```
[wp-pic slug="wp-plugin-info-card" layout="wordpress"]
```

### scheme

Select a card color scheme.  Available schemes are `scheme1` through `scheme14`. The default scheme can be set in the admin settings.

```
[wp-pic slug="wp-plugin-info-card" scheme="scheme14"]
```

### image

Designate an image that will take the place of a plugin's default banner.

```
[wp-pic slug="wordpress-seo" image="http//www.mywebsite/custom-image.jpg"]
```

### align

Set the alignment of the info card. Values can be:

- center
- left
- right

### containerid

Set the container ID of the plugin wrapper. 

The default is: `default: wp-pic-PLUGIN-SLUG`.

### margin

Set the margin for the info card. The default is no margin.

```
[wp-pic slug="wordpress-seo" align="right" margin="0 0 0 20px"]
```

### clear

Whether to clear the float of the container. Default is empty.

Choices are:

- below
- after

```
[wp-pic slug="wordpress-seo" clear="after"]
```

### expiration

By default, the info card are cached at 720 seconds, so as to not ping the WordPress plugin API in excess.

You can change this expiration when outputting your cards.

```
[wp-pic type="theme" slug="zerif-lite" expiration="60"]
```

### ajax

Whether to load the plugin in via Ajax.

Choices are: `yes` and `no`.

### custom

Whether to output any strings associated with a plugin or theme.

For plugins: *url, name, icons, banners, version, author, requires, rating, num_ratings, downloaded, last_updated, download_link*

For themes: *url, name, version, author, screenshot_url, rating, num_ratings, downloaded, last_updated, homepage, download_link*
