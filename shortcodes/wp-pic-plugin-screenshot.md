---
slug: wp-pic-plugin-screenshot
title: "wp-pic-plugin-screenshot"
products: [wp-plugin-info-card]
sections: ["shortcodes"]
tags: []
status: publish
---

You can use the plugin screenshots shortcode to display a plugin card with screenshots anywhere shortcodes are supported.

Here is an example of the shortcode in use, using default settings.

```markup
[wp-pic-plugin-screenshots slug="simple-comment-editing"]
```

The following are the parameters for the shortcode:

### unique_id

The Unique ID surrounding the card's HTML structure. This is randomized if omitted.

### slug (required)

The plugin slug for the WordPress.org asset.

### icon_style

Can be:

- **none** - No icon style
- **border** - Icon with a border
- **bw** - Black & White icon

### enable_rounded_icon

Determine if you would like a rounded icon or not for the plugin icon.

Can be:

- **true** - Rounded icon
- **false** - Square icon

### color_theme

Choose from several built-in color themes.

Can be:

- default
- blossom
- crimson
- velvet
- dark
- light
- feathers
- caramel

### custom_colors

Set to **true** to override the built-in color themes and provide your own custom colors.

### plugin_title

Override the plugin's title with something more custom or shorter than the original title.

### enable_context_menu

Enable or disable the context menu that shows extra information about the plugin.

Can be:

- true
- false

### enable_screenshots

Enable or disable the screenshots that display with the plugin.

Can be:

- true
- false

### align

Align the output according to the theme. Can be:

- center
- wide
- full

### color_background

Hex code for the background of the plugin container.

### color_text

Hex code for the main text color.

### color_border

The hex code for the border color of the plugin container.

### color_menu_border

The hex code for the border of the contextual menu.

### color_menu

The hex code for the contextual menu color.

### color_menu_hover

The hex code for the contextual menu color on hover.

### color_menu_text

The hex code for the contextual menu text color.

### color_menu_text_hover

The hex code for the contextual menu text color on hover.

### color_screenshots_background

The hex code for the background of the screenshots section.

### color_screenshots_border

The hex code for the border of the screenshots section.

### color_screenshots_arrow_background

The hex code for the screenshot arrows background color.

### color_screenshots_arrow_background_hover

The hex code for the screenshots arrows background color on hover.

### color_screenshots_arrow

The hex code for the arrow color.

### color_screenshots_arrow_hover

The hex code for the arrow color on hover.

### color_star

The hex code for the star color when showing ratings.

### color_meta_background

The hex code background color for the meta section.

### color_meta_text

The hex code for the text color of the meta sectioin.

### skip_animated_gifs

Disable animated gifs from showing in the screenshots. This can help speed up loading time.

```
[wp-pic-plugin-screenshots slug="highlight-and-share" skip_animated_gifs="true"]
```
