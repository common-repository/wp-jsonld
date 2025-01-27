=== wp-jsonld ===

Contributors: Benjamin Marwell
Original Authors: Mikko Piippo, tlattu
Donate link:
Tags: json-ld, markup, schema, rich snippets, structured data, microdata, SEO,schema.org,schema markup,JSON
Requires at least: 4.0
Tested up to: 4.4
Stable tag: 0.3.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

wp-jsonld is the continuation of the simplest solution to add valid schema.org microdata as JSON-LD-script to your blog posts and articles.

== Description ==

= Why this plugin exists =
Original Plugin (discontinued): https://de.wordpress.org/plugins/json-ld-for-article/

Sadly, the original plugin is not being developed anymore. So I decided to fix some bugs like invalid markup,
    missing tags, putting objects into fields instead of just URLs for images, and implementing for more than just
    articles.

Also, this plugin plays nicely with [YASR - yet another star rating](https://de.wordpress.org/plugins/yet-another-stars-rating/). It will
remove yasr's invalid jsonld-syntax and instead use YASRs rating.

All requests are being cached and purged on page update/edit etc.

[![Stories in Ready](https://badge.waffle.io/bmhm/wp-jsonld.png?label=ready&title=Ready)](https://waffle.io/bmhm/wp-jsonld)

= Original description =
Search engines such as Google are using structured data markup in many ways—for example, to create rich snippets in search results. Search results with rich snippets will improve your click through rates and increase the number of visitors on your website.

It has been a tedious task to add the complicated Schema.org markup to your website - sometimes it wasn’t even possible due to technical constraints. Now, thanks to **JSON-LD**, almost any website can enjoy the benefits of structured data. For WordPress users it’s even easier thanks to this plugin.

JSON-LD for Article is simply the easiest solution to create valid schema.org microdata markup on your Wordpress site automatically from your web content and its metadata. All you need to do is install and activate the plugin, and it will generate JSON-LD markup of your posts that Google and other search engines can use for rich snippets using the schema.org for articles.

Some WP themes include traditional schema.org markup embedded in the html code the theme produces. If you are using one of these themes, this plugin is probably not necessary. If the markup produced by the theme contradicts the data specified in the JSON-LD, the added information might be not be helpful at all. Thus you should check the markup provided by the theme before adding possibly unnecessary JSON-LD to your site.

On the other hand, if you use a custom theme, it is easier to use the functionality provided by the plugin than to invent the wheel again and add the markup in html. Very often, this leads to html code that is difficult to read and is not valid structural markup according to Google’s validator. 

Our plugin:

* Helps your site to earn rich snippets in Google’s SERP.
* Does not depend on other plugins or external code.
* Is simple to install: plug-and-play, no need to configure anything.


== Installation ==

The easiest way to install the plugin is to use the WP built-in menu for finding and installing new plugins directly from the WordPress repositories.

If you need to install this using FTP or SFTP, you should follow these steps:

1. Upload all files recursively to the `/wp-content/plugins/` directory using your favorite FTP client.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. That’s it.

**Compatibility.** This version requires php 5.4 for some options of json\_encode. If you encounter any problems with the plugin you should check your web hotel’s php version.

== Frequently Asked Questions ==
**How do I test if this plugin works?** Go to https://developers.google.com/structured-data/testing-tool/ and enter the URL of one of your articles / blog posts.

**Are Authors (Person) markups supported on author pages?** Soon.

**Does this plugin produce valid markup?** According to Google, yes.

**Where is the logo taken from?** Currently it uses https://logo.clearbit.com/&lt;url&gt;. This will change soon.

**Does this plugin X?** Most probably, it does not. This plugin simply adds to the footer of your single post views valid JSON-LD filled with the data from the WP database. You should not see anything new on the page - the JSON-LD can be seen only in the source code of the web page.

**Why should I install this plugin?** Installing this plugin is the easiest way to add structured data to your blog. The plugin automatically creates the JSON-LD according to Google’s specification. 

**Does this plugin improve my SEO rankings?** We cannot promise it - but installing this plugin is in any case a step in right direction.

== Screenshots ==

Screenshots will be added soon.

== Changelog ==

= 0.3.2 =
* Find correct front page.

= 0.3.1 =
* updated type so release could be pushed.

= 0.3.0 =
* Use transients for caching.
* Use tag 'aggregateRating' if YSSR is installed.

= 0.2.0 =
* Extended the functionality a bit and completely refactored the code to make it much more readable.

= 0.1 =
*  This is a fully functional version based on the idea of minimum viable product. It delivers what it promises, without any bells and whistles. Some people might regard this as a beta version :)
