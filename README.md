# Utopian Images

This bullet-proof thumbnail script finds all possible sources for a post or term's image including WP's native thumbnail, attachments, object content and meta

## Getting Started

Please refer to Utopian Images' <a href="#">official plugin page</a> to download the plugin


### Installing

Once the plugin is activated, you can use the plugin's function inside your theme's files. Because the plugin returns a url, this function should be used in replacement of img src values. The following example gives you an idea of how the function should be used.

```php
<img src="<?php
if (function_exists('uwp_thumb')) {echo uwp_thumb(array('id' => '111', 'type' => 'post');}
?>" />
```

The function accepts an optional array of arguments which for now include 'id', and 'type'. These are only needed if you're calling the function outside of the loop.

Options can be found in 'Settings-> Utopian Images. Please refer to the FAQ section to understand these options.


## FAQ


### What does Thumbnail Source Priorities option do?
There are four sources that Utopian Images checks to find an object's image. Because the plugin stops looking once it finds an image, you may want to reorder the sources if you have preferences about which are used. This is done by clicking and dragging on the options. The default setting is ideal for most sites.


### What does the Comma-Separated Meta Key Matches option do?
One of the places that the plugin looks for an object's image is in your site's meta data. Using comma's to seperate, you can add keywords to be used for matches against the meta key names in your database. You don't have to use the entire meta key, just a search word that can be found within it. The default setting is ideal for most sites.



## Versioning

For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Paul Sandberg** - *Initial work* - [uwpweb](https://github.com/uwpweb)

## License

Utopian Images is licensed under the GPL v3 or later.

> This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License, version 2, as published by the Free Software Foundation.

> This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

> You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA

A copy of the license is included in the root of the plugin’s directory. The file is named `LICENSE`.


### Licensing

The WordPress Plugin Boilerplate is licensed under the GPL v2 or later; however, if you opt to use third-party code that is not compatible with v2, then you may need to switch to using code that is GPL v3 compatible.

For reference, [here's a discussion](http://make.wordpress.org/themes/2013/03/04/licensing-note-apache-and-gpl/) that covers the Apache 2.0 License used by [Bootstrap](http://twitter.github.io/bootstrap/).
