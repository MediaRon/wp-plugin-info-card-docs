---
title: "wp-pic-query"
sections: [Shortcodes]
status: publish
---

# wp-pic-query

The `wp-pic-query` shortcode is used to output a set of a plugin based on a query you specify.

All of the `wp-pic` shortcode attributes apply as well. You may need to change `type` to 'theme' if you are querying for themes.

{% content-ref url="wp-pic.md" %}
[wp-pic.md](wp-pic.md)
{% endcontent-ref %}

Here are the available parameters.

### search (default empty)

Search the plugin or theme directory for a keyword. Example of retrieving plugins that have to do with higlighting.

```
[wp-pic-query search="highlight"]
```

### tag (default empty, can be comma-separated)

Search for a specific plugin or theme tag.

{% code overflow="wrap" %}
```
[wp-pic-query tag="dark,four-columns" per_page="4" type="theme" layout="wordpress" align="center" ajax="yes" cols="2"]
```
{% endcode %}

### author (default empty, WordPress.org username)

Retrieve a list of plugins or themes based on the .org username.

{% code overflow="wrap" %}
```
[wp-pic-query author="automattic" per_page="6" type="plugin" layout="wordpress" align="center" ajax="yes" cols="2"]
```
{% endcode %}

### user (default empty, WordPress.org username)

Retrieve a user's favorite plugins.

{% code overflow="wrap" %}
```
[wp-pic-query user="briKou" per_page="4" type="plugin" layout="wordpress" align="center" ajax="yes" cols="2"]
```
{% endcode %}

### browse (default empty)

Browse, if specified, can have the following values.

* featured
* popular
* updated
* favorites

{% code overflow="wrap" %}
```
[wp-pic-query browse="popular" per_page="6" type="plugin" layout="card" margin="1rem" ajax="yes" cols="2"]
```
{% endcode %}

### per\_page (default 24)

How many results should be returned.

{% code overflow="wrap" %}
```
[wp-pic-query tag="buddypress" per_page="2" type="theme" layout="large" align="center" align="center"]
```
{% endcode %}

### cols (default 2)

This is an appearance attribute. Choose from 1 to 3 columns for the output.

### col\_gap

The gap between columns in pixels.

### row\_gap

The gap between rows in pixels.

### {slug}={title} or {slug}="false"

A slug can be set in the shortcode attributes to override the title or disable the plugin from displaying.

Simply use the plugin or theme slug in the shortcode attributes.

Here's an example:

{% code overflow="wrap" %}
```
[wp-pic-query author="ronalfy" per_page="6" type="plugin" layout="wordpress" align="center" ajax="yes" cols="2" alerts-dlx="Alerts DLX" wp-ajaxify-comments="false" simple-comment-editing="Conversational Editing"]
```
{% endcode %}
