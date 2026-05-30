---
title: "wp-pic-badges"
sections: [Shortcodes]
status: publish
---

# wp-pic-badges

### Overview

The `[wp-pic-badges]` shortcode allows you to display WordPress.org profile badges on your site. You can display either static badges (manually selected) or dynamic badges (automatically fetched from a WordPress.org profile).

{% hint style="warning" %}
This feature requires Dashicons. If you have a plugin that disables Dashicons, such as Perfmatters, please re-enable it for this feature to work.
{% endhint %}

#### Features

* **Static Badges**: Manually select and display specific badges
* **Dynamic Badges**: Automatically fetch and display badges from any WordPress.org profile
* **Flexible Layout**: Control columns, spacing, alignment, and layout style
* **Customizable Styling**: Adjust font size, colors, and spacing
* **Lazy Loading**: Dynamic badges load efficiently with automatic caching
* **Accessibility**: Built-in ARIA labels and semantic HTML

***

### Basic Usage

#### Static Badges

Display manually selected badges:

```
[wp-pic-badges badges="badge-code,badge-plugins,badge-design-contributor"]
```

#### Dynamic Badges

Display badges from a WordPress.org profile:

```
[wp-pic-badges type="dynamic" author_slug="ronalfy"]
```

***

### Shortcode Syntax

```
[wp-pic-badges attribute="value" attribute2="value2" ...]
```

All attributes are optional. If not specified, default values will be used.

***

### Attributes Reference

#### Core Attributes

| Attribute     | Type   | Default  | Description                                                                       |
| ------------- | ------ | -------- | --------------------------------------------------------------------------------- |
| `type`        | string | `static` | Badge type: `static` (manual selection) or `dynamic` (from WordPress.org profile) |
| `badges`      | string | `''`     | Comma-separated list of badge class names (for static type only)                  |
| `author_slug` | string | `''`     | WordPress.org username (for dynamic type only)                                    |

#### Layout Attributes

| Attribute      | Type    | Default      | Description                                                                |
| -------------- | ------- | ------------ | -------------------------------------------------------------------------- |
| `badge_layout` | string  | `grid`       | Display layout: `grid` (structured columns) or `flex` (fluid wrapping)     |
| `cols`         | integer | `2`          | Number of columns in the grid (1, 2, or 3) - only applies to `grid` layout |
| `layout`       | string  | `horizontal` | Badge item layout style: `horizontal` or `centered`                        |
| `align`        | string  | `center`     | Alignment: `left`, `center`, or `right`                                    |
| `col_gap`      | integer | `20`         | Column gap in pixels                                                       |
| `row_gap`      | integer | `20`         | Row gap in pixels                                                          |

#### Display Attributes

| Attribute       | Type    | Default   | Description                                        |
| --------------- | ------- | --------- | -------------------------------------------------- |
| `hide_heading`  | boolean | `false`   | Hide badge headings (set to `true` or `1` to hide) |
| `heading_color` | string  | `#000000` | Heading text color (hex code)                      |
| `base_size`     | integer | `16`      | Base font size in pixels                           |

#### Advanced Attributes

| Attribute   | Type   | Default | Description                                 |
| ----------- | ------ | ------- | ------------------------------------------- |
| `anchor`    | string | `''`    | Custom anchor ID for the wrapper element    |
| `unique_id` | string | `''`    | Unique identifier (auto-generated if empty) |

***

### Usage Examples

#### Example 1: Basic Static Badges

Display three badges in a 2-column grid:

```
[wp-pic-badges badges="badge-code,badge-plugins,badge-design-contributor" cols="2"]
```

#### Example 2: Dynamic Badges from Profile

Display badges from a WordPress.org profile:

```
[wp-pic-badges type="dynamic" author_slug="ronalfy" cols="3"]
```

#### Example 3: Custom Layout and Styling

Customize columns, spacing, and colors:

```
[wp-pic-badges 
    badges="badge-code,badge-plugins,badge-design-contributor"
    cols="3"
    col_gap="30"
    row_gap="20"
    layout="centered"
    base_size="18"
    heading_color="#333333"
    align="center"
]
```

#### Example 4: Hide Badge Headings

Display badges without their headings:

```
[wp-pic-badges badges="badge-code,badge-plugins" hide_heading="true"]
```

#### Example 5: Single Column Layout

Display badges in a single column:

```
[wp-pic-badges badges="badge-code,badge-plugins,badge-design-contributor" cols="1"]
```

#### Example 6: Badges with Overlay Modifier

Some badges include the `has-overlay` modifier for special styling:

```
[wp-pic-badges badges="badge-code-committer has-overlay,badge-design has-overlay" cols="2"]
```

#### Example 7: Flex Layout

Display badges in a fluid, wrapping flex layout (badges wrap naturally based on available space):

```
[wp-pic-badges badges="badge-code,badge-plugins,badge-design-contributor" badge_layout="flex"]
```

#### Example 8: Flex Layout with Custom Spacing

Use flex layout with custom gap spacing:

```
[wp-pic-badges 
    badges="badge-code,badge-plugins,badge-design-contributor"
    badge_layout="flex"
    col_gap="25"
    row_gap="15"
    align="center"
]
```

***

### Available Badges

The following badges are available for use with the `badges` attribute. Badges are sorted alphabetically by label.

| Badge Class                          | Label                      |
| ------------------------------------ | -------------------------- |
| `badge-accessibility has-overlay`    | Accessibility Team         |
| `badge-accessibility-contributor`    | Accessibility Contributor  |
| `badge-bbpress has-overlay`          | BBPress Team               |
| `badge-bbpress-contributor`          | BBPress Contributor        |
| `badge-buddypress has-overlay`       | BuddyPress Team            |
| `badge-buddypress-contributor`       | BuddyPress Contributor     |
| `badge-campus-connect-participant`   | Campus Connect Participant |
| `badge-code`                         | Core Contributor           |
| `badge-code-committer has-overlay`   | Core Team                  |
| `badge-community-contributor`        | Community Contributor      |
| `badge-core-ai-contributor`          | Core AI Contributor        |
| `badge-core-ai-team has-overlay`     | Core AI Team               |
| `badge-credits-graduate`             | Credits Graduate           |
| `badge-credits-mentor`               | Credits Mentor             |
| `badge-design has-overlay`           | Design Team                |
| `badge-design-contributor`           | Design Contributor         |
| `badge-documentation has-overlay`    | Documentation Team         |
| `badge-documentation-contributor`    | Documentation Contributor  |
| `badge-hosting has-overlay`          | Hosting Team               |
| `badge-hosting-contributor`          | Hosting Contributor        |
| `badge-marketing has-overlay`        | Marketing Team             |
| `badge-marketing-contributor`        | Marketing Contributor      |
| `badge-media-corps-contributor`      | Media Corps Contributor    |
| `badge-media-corps-team has-overlay` | Media Corps Team           |
| `badge-meta-contributor`             | Meta Contributor           |
| `badge-mobile`                       | Mobile Contributor         |
| `badge-openverse has-overlay`        | Openverse Team             |
| `badge-openverse-contributor`        | Openverse Contributor      |
| `badge-organizer`                    | WordCamp Organizer         |
| `badge-pattern-author`               | Patterns Author            |
| `badge-patterns-team`                | Patterns Team              |
| `badge-performance-contributor`      | Performance Contributor    |
| `badge-performance-team has-overlay` | Performance Team           |
| `badge-photo-contributor`            | Photo Contributor          |
| `badge-photos-team`                  | Photos Team                |
| `badge-playground`                   | Playground Developer       |
| `badge-playground-contributor`       | Playground Contributor     |
| `badge-plugins`                      | Plugin Developer           |
| `badge-plugins-reviewer has-overlay` | Plugins Team               |
| `badge-security-contributor`         | Security Team              |
| `badge-security-team`                | Security Team              |
| `badge-speaker`                      | WordCamp Speaker           |
| `badge-support-contributor`          | Support Contributor        |
| `badge-sustainability-contributor`   | Sustainability Contributor |
| `badge-sustainability-team`          | Sustainability Team        |
| `badge-test has-overlay`             | Test Team                  |
| `badge-test-contributor`             | Test Contributor           |
| `badge-themes`                       | Theme Developer            |
| `badge-themes-reviewer has-overlay`  | Themes Team                |
| `badge-tide has-overlay`             | Tide Team                  |
| `badge-tide-contributor`             | Tide Contributor           |
| `badge-training has-overlay`         | Training Team              |
| `badge-training-contributor`         | Training Contributor       |
| `badge-translation-contributor`      | Translation Contributor    |
| `badge-translation-editor`           | Translation Editor         |
| `badge-wordcamp-volunteer`           | WordCamp Volunteer         |
| `badge-wordpress-tv-contributor`     | WordPress TV Contributor   |
| `badge-wp-cli has-overlay`           | WP CLI Team                |
| `badge-wp-cli-contributor`           | WP CLI Contributor         |

#### Badge Class Modifiers

* **`has-overlay`**: Included automatically in the badge class string for certain badges (typically team badges) to provide special overlay styling. When using these badges, include the full class string as shown in the table above.

***

### Tips and Best Practices

#### Badge Selection

* **Multiple Badges**: Separate badge class names with commas (no spaces around commas)
* **Case Sensitivity**: Badge class names are case-sensitive
* **Invalid Badges**: Invalid badge classes will be automatically filtered out
* **Modifiers**: Include modifiers like `has-overlay` as part of the badge class string

#### Layout Tips

* **Grid vs Flex**:
  * **Grid Layout** (`badge_layout="grid"`): Use for structured, column-based layouts. Supports 1, 2, or 3 columns via the `cols` attribute. Best for consistent, organized badge displays.
  * **Flex Layout** (`badge_layout="flex"`): Use for fluid, wrapping layouts. Badges wrap naturally based on available space. Best for responsive designs where badges should adapt to container width. The `cols` attribute is ignored in flex layout.
* **Columns**: For grid layout, use 1 column for narrow spaces, 2-3 columns for wider areas
* **Spacing**: Adjust `col_gap` and `row_gap` to match your site's design (works for both grid and flex layouts)
* **Alignment**: Use `align="center"` for centered layouts, `align="left"` or `align="right"` for edge alignment

#### Dynamic Badges

* **Caching**: Dynamic badges are automatically cached for performance
* **Loading**: A loading skeleton appears while badges are being fetched
* **Updates**: Badge data is refreshed automatically when cache expires (14 days)
* **Author Slug**: Use the WordPress.org username (slug), not the display name

#### Performance

* **Static Badges**: Load immediately (no API calls)
* **Dynamic Badges**: Use lazy loading and multi-layer caching for optimal performance
* **Multiple Instances**: You can use multiple shortcode instances on the same page

***

### Common Use Cases

#### Showcase Your Contributions

Display your WordPress.org badges on your personal website:

```
[wp-pic-badges type="dynamic" author_slug="your-username" cols="3"]
```

#### Highlight Team Members

Show badges for team members:

```
[wp-pic-badges badges="badge-code,badge-plugins,badge-design-contributor" cols="2" layout="centered"]
```

#### Minimal Badge Display

Show badges without headings for a cleaner look:

```
[wp-pic-badges badges="badge-code,badge-plugins" hide_heading="true" cols="1"]
```

#### Custom Styled Badges

Match your site's color scheme:

```
[wp-pic-badges 
    badges="badge-code,badge-plugins"
    heading_color="#1e73be"
    base_size="18"
    col_gap="25"
    row_gap="15"
]
```

***

### Troubleshooting

#### Badges Not Displaying

1. **Check Badge Names**: Ensure badge class names are spelled correctly and match the available badges list
2. **Check Author Slug**: For dynamic badges, verify the WordPress.org username is correct
3. **Invalid Classes**: Invalid badge classes are automatically filtered out

#### Layout Issues

1. **Column Count**: For grid layout, ensure `cols` is set to 1, 2, or 3. Note: `cols` attribute is ignored in flex layout.
2. **CSS Conflicts**: Check for theme or plugin CSS conflicts
3. **Container Width**: Ensure the container has sufficient width for the column layout (grid) or wrapping (flex)
4. **Layout Type**: Verify `badge_layout` is set to either `grid` or `flex` (defaults to `grid` if invalid)

#### Dynamic Badge Loading

1. **Loading Skeleton**: A loading skeleton appears while badges are being fetched
2. **Cache**: Badge data is cached for 14 days; wait for cache expiration or clear cache to refresh
3. **Network Issues**: Check network connectivity if badges fail to load

***

### Technical Details

#### HTML Structure

The shortcode generates a container with the following structure:

**Grid Layout:**

```html
<div class="wppic-badges-grid is-grid align{center|left|right} layout-{horizontal|centered} cols-{1|2|3}" id="{uniqueId}">
    <style>
        #{uniqueId}.wppic-badges-grid {
            --wppic-grid-row-gap: {rowGap}px;
            --wppic-grid-col-gap: {colGap}px;
            --wppic-base-size: {baseSize}px;
            --wppic-heading-color: {headingColor};
        }
    </style>
    <!-- Badge HTML -->
</div>
```

**Flex Layout:**

```html
<div class="wppic-badges-flex is-flex align{center|left|right} layout-{horizontal|centered}" id="{uniqueId}">
    <style>
        #{uniqueId}.wppic-badges-flex {
            --wppic-flex-gap: {gap}px;
            --wppic-base-size: {baseSize}px;
            --wppic-heading-color: {headingColor};
        }
    </style>
    <!-- Badge HTML -->
</div>
```

#### CSS Classes

* `wppic-badges-grid` - Base container class for grid layout
* `wppic-badges-flex` - Base container class for flex layout
* `is-grid` - Grid layout indicator (only for grid layout)
* `is-flex` - Flex layout indicator (only for flex layout)
* `align{center|left|right}` - Alignment modifier
* `layout-{horizontal|centered}` - Badge item layout style modifier
* `cols-{1|2|3}` - Column count modifier (only for grid layout)
* `has-no-title` - Applied when `hide_heading` is true

#### CSS Variables

The following CSS variables are set for customization:

**Grid Layout:**

* `--wppic-grid-row-gap` - Row spacing in pixels
* `--wppic-grid-col-gap` - Column spacing in pixels
* `--wppic-base-size` - Base font size in pixels
* `--wppic-heading-color` - Heading text color (hex code)

**Flex Layout:**

* `--wppic-flex-gap` - Gap spacing in pixels (combines row and column gap)
* `--wppic-base-size` - Base font size in pixels
* `--wppic-heading-color` - Heading text color (hex code)

***

### Support

For issues, feature requests, or questions, please contact [support](https://dlxplugins.com/support/).
