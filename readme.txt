=== Good old Share ===
Contributors: whiletrue
Donate link: http://www.whiletrue.it/
Tags: facebook, twitter, facebook share, twitter share, facebook share button, twitter share button, linkedin, google +1, +1, google share, google plus share, pinterest, google buzz, buzz, digg, flattr, stumbleupon, hyves, links, post, page, mail, email, reddit, tipy, tumblr, buffer, pinzout, shortcode, youtube, print, rss, bitcoin, litecoin, specificfeeds, draugiem, frype
Requires at least: 2.9+
Tested up to: 4.2
Stable tag: 1.0.1

Puts Facebook, Twitter, LinkedIn, Google "+1", Pinterest, Tumblr and other social share buttons of your choice above or below your posts.

== Description ==
This plugin shows Facebook, Twitter, LinkedIn, Google "+1", Pinterest and other popular social share buttons above or below your posts.
Easy customization of active buttons and position in the Settings menu.

In contrast to several other sharing plugin, this one aims to use only original code provided by any social network.
There is no other service in the middle, you are not required to register or get a key to use it. Enjoy!

Facebook Like, Twitter and Google +1 social share buttons are loaded by default. 
Other buttons, including Digg, Facebook Share, Flattr, LinkedIn, Pinterest, Bitcoin, Litecoin, Stumbleupon, Youtube, Hyves, Print, Email, RSS, Reddit, Tipy, Tumblr, Buffer, Pinzout, SpecificFeeds, Draugiem.lv (Frype.com) can be added through the `Settings->Good old Share` menu.

Please be careful when selecting the `Show buttons in these pages` options : it can interact badly with other slide/fade/carousel/sidebar active plugins.

= Shortcode =

If you want to place the active buttons only in selected posts, use the [good_old_share] shortcode.

If you want to place only one share button, add the *button* attribute to the shortcode, e.g.:

* [good_old_share button="facebook_like"]
* [good_old_share button="twitter"]
* [good_old_share button="linkedin"]
* [good_old_share button="pinterest"]
* [good_old_share button="google1"]
* [good_old_share button="digg"]
* [good_old_share button="stumbleupon"]
* [good_old_share button="reddit"]
* [good_old_share button="flattr"]
* [good_old_share button="tumblr"]
* [good_old_share button="facebook_share"]
* and so on...

Please note that in order to place single share buttons, they have to be active in the plugin settings page.

= Selective disable =

If you want to hide the share buttons inside selected posts, set a "good_old_share_disable" custom field with value "yes".

To do so e.g. on a page: open the WordPress backend, go to Pages, click on the Page title to enter the Page edit screen. Then you can add the custom field, [as explained here](http://www.carriedils.com/how-to-create-custom-fields-in-wordpress/ "How to Create Custom Fields in WordPress").

= Reference =

This plugin gives you the features of the former 3.3 release of the "Really simple Share" plugin.

For more info: [www.whiletrue.it](http://www.whiletrue.it/really-simple-share-wordpress-plugin/ "www.whiletrue.it")

Do you like this plugin? Give a chance to our other works:

* [Most and Least Read Posts](http://www.whiletrue.it/most-and-least-read-posts-widget-for-wordpress/ "Most and Least Read Posts")
* [Tilted Tag Cloud Widget](http://www.whiletrue.it/tilted-tag-cloud-widget-per-wordpress/ "Tilted Tag Cloud Widget")
* [Reading Time](http://www.whiletrue.it/reading-time-for-wordpress/ "Reading Time")

Also, take a look at [the current version of Really simple Share](https://wordpress.org/plugins/really-simple-facebook-twitter-share-buttons/ "Really simple Share")

== Installation ==
Best is to install directly from WordPress. If manual installation is required, please make sure to put all of the plugin files in a folder named `good-old-share` (not two nested folders) in the plugin directory, then activate the plugin through the `Plugins` menu in WordPress.

== Frequently Asked Questions ==

= The settings page seems corrupted, some buttons labels are missing. How to solve it? =

Sometimes the options get corrupted after several plugin updates. 
Click the Reset button (on the lowest right of the plugin settings page) to give the plugin a fresh start. 
Please take a note of your plugin configuration before resetting the options, or remember the data you want to put back in.

= What's the difference between Facebook Like and Share buttons? =
Facebook Like is the official Button actively supported by Facebook.
On 18th July 2012 Facebook dropped support for the (old and long time deprecated) Share button, so this button has been removed from the plugin and replaced with an externali link with no counter.

= Why users can't choose which image to share when using Facebook Like button ? =
This is an automated Facebook behaviour: clicking Facebook Like the user can't choose each time which image to share, 
but you can set the right image inside the code using the 
<a href="http://developers.facebook.com/docs/reference/plugins/like/">Open Graph Tag</a> og:image.

= When I activate the plugin it messes up with other plugins showing post excerpts in different ways (fade, carousel, sidebar). What can I do? =
Uncheck all the "Show buttons in these pages" options in the `Settings->Good old Share` menu, except for "Single posts".
This way all the share buttons should disappear, except the one displayed beside the post in every Single post page.

= Is it possible to modify the style/css of the buttons? =
Yes, every button has its own div class (e.g. "good_old_share_twitter") for easy customization inside the theme css files.
Plus, the div surrounding all buttons has its own class "good_old_share". 
If you want to override default styling of the buttons, check the `disable default styles` option add your style rules inside your css theme file.

= Is it possible to show the buttons anywhere inside my theme, using a PHP function? =
Yes, you can call this PHP function:
`<?php echo good_old_share_publish($link='', $title=''); ?>` 
You can pass the share link and the title as parameters.
You shouldn't leave the parameters blank, unless the code is put inside the WP loop.
For example, use this code to create buttons linking to the website home page:
`<?php echo good_old_share_publish(get_bloginfo('url'), get_bloginfo('name'));  ?>`

= Sometimes the Pinterest PinIt button doesn't appear in some posts. =
The PinIt button requires some media to share, so it only shows up when the post contains at least one image.

= I've cheched the "show counter" option in the Settings page, but sometimes the Pinterest PinIt button's counter doesn't appear. =
The PinIt counter only appear if the post has been shared at least once. Also, the refresh time for the PinIt counter could be long. 

== Screenshots ==
1. Sample content, activating the Facebook Share and Twitter buttons  
2. Options available in the Settings menu 


== Changelog ==

= 1.0.1 =
* Plugin tested up WordPress 4.2

= 1.0 =
Initial release


== Upgrade Notice ==

= 1.0 =
Initial release
