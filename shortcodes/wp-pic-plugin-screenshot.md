---
description: Display a plugin card with screenshots.
---

# wp-pic-plugin-screenshot

You can use the plugin screenshots shortcode to display a plugin card with screenshots anywhere shortcodes are supported.

Here is an example of the shortcode in use, using default settings.

```markup
[wp-pic-plugin-screenshots slug="simple-comment-editing"]
```

The following are the parameters for the shortcode:

### unique\_id

The Unique ID surrounding the card's HTML structure. This is randomized if omitted.

### slug (required)

The plugin slug for the WordPress.org asset.

### icon\_style

Can be:

* **none** - No icon style
* **border** - Icon with a border
* **bw** - Black & White icon

### enable\_rounded\_icon

Determine if you would like a rounded icon or not for the plugin icon.

Can be:

* **true** - Rounded icon
* **false** - Square icon

### color\_theme

Choose from several built-in color themes.

Can be:

* default
* blossom
* crimson
* velvet
* dark
* light
* feathers
* caramel

### custom\_colors

Set to **true** to override the built-in color themes and provide your own custom colors.

### plugin\_title

Override the plugin's title with something more custom or shorter than the original title.

### enable\_context\_menu

Enable or disable the context menu that shows extra information about the plugin.

Can be:

* true
* false

### enable\_screenshots

Enable or disable the screenshots that display with the plugin.

Can be:

* true
* false

### align

Align the output according to the theme. Can be:

* center
* wide
* full

### color\_background

Hex code for the background of the plugin container.

### color\_text

Hex code for the main text color.

### color\_border

The hex code for the border color of the plugin container.

### color\_menu\_border

The hex code for the border of the contextual menu.

### color\_menu

The hex code for the contextual menu color.

### color\_menu\_hover

The hex code for the contextual menu color on hover.

### color\_menu\_text

The hex code for the contextual menu text color.

### color\_menu\_text\_hover

The hex code for the contextual menu text color on hover.

### color\_screenshots\_background

The hex code for the background of the screenshots section.

### color\_screenshots\_border

The hex code for the border of the screenshots section.

### color\_screenshots\_arrow\_background

The hex code for the screenshot arrows background color.

### color\_screenshots\_arrow\_background\_hover

The hex code for the screenshots arrows background color on hover.

### color\_screenshots\_arrow

The hex code for the arrow color.

### color\_screenshots\_arrow\_hover

The hex code for the arrow color on hover.

### color\_star

The hex code for the star color when showing ratings.

### color\_meta\_background

The hex code background color for the meta section.

### color\_meta\_text

The hex code for the text color of the meta sectioin.

### skip\_animated\_gifs

Disable animated gifs from showing in the screenshots. This can help speed up loading time.

{% code overflow="wrap" %}
```
[wp-pic-plugin-screenshots slug="highlight-and-share" skip_animated_gifs="true"]
```
{% endcode %}

