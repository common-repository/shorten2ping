=== Shorten2Ping ===
Contributors: samuelaguilera
Donate link: http://bit.ly/s2pdonate
Tags: ping.fm, bit.ly, ping, twitter, facebook, linkedin, plurk, su.pr, yourls, is.gd, j.mp, cli.gs, wp.me, wpmu
Requires at least: 2.7
Tested up to: 3.3.1
Stable tag: 1.4.8

Sends <strong>status</strong> updates to Ping.fm everytime you publish a post, using your own domain, bit.ly, wp.me, su.pr, is.gd and others for shortened permalinks.

== Description ==

<strong>IMPORTANT!!: At present Seesmic has blocked the API key for this plugin, you can <a href="http://ur1.es/djjSqf">read more here</a>. So I have added support for using email notification, this is working for some users and not for others. Sorry but I can't do more about this, so blame to Seesmic not me.</strong>

<strong>UPDATE (2011/08/27): Ping.fm support will be removed in a future version of this plugin.</strong>

Sends <strong>status</strong> updates to <a href="http://ping.fm">Ping.fm</a> (this means you can update Twitter, Facebook, LinkedIn, Plurk, and many others at once) everytime you publish a post. Using many shorteners or even your own domain for shortened permalinks. So this way you can send status to many sites at once if you have a Ping.fm account or send only to Twitter if you prefer that.

If you find it useful, please consider to make a <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=8801680">donation</a> to Shorten2Ping's author (any amount will be appreciated).

= Features =

* Send new posts notifications to <strong>Ping.fm</strong> service (account required).
* <strong>Avoids to ping again when editing</strong> previously pinged post or even when editing an old post not pinged before.
* Option to choose between <strong>bit.ly, tr.im, YOURLS, su.pr, is.gd, j.mp, wp.me, cli.gs or even you own domain</strong> for shortened permalinks.
* Option to turn off notification or shortener service. Now <strong>you can use Shorten2Ping only for notification</strong> if your domain is already short enough for you, <strong>or use only to get shortened urls for your posts.</strong>
* <strong>Stores created shortened permalink</strong> in a post meta field (used for template integration).
* <strong>Using <code>rel="shortlink"</code></strong> like in wp.me http://wp.me/sf2B5-shorten, creating auto-discovery link tag for the short link on single post page header.
* You can use a <strong>template tag for showing visitors the short URL</strong> (using the same rel attribute as above for the shortened permalink).
* <strong>Locale support</strong>. Now available in English, Spanish, Italian and Traditional Chinese (zh_TW). See translation section for more info.
* WPMU compatible (you can have different settings for each blog).
* <strong>Simple</strong>, fast, and useful :)

= Requirements =

* PHP 5.x with CURL and JSON enabled (maybe works too in PHP4, but not tested and not supported by me).
* Your hosting provider must allow the use of PHP mail() function if you choose 'Ping.fm email' notification method.
* WordPress 2.7.x or higher (maybe would work on older WP, but not tested and not supported by me).
* Required your own account for the third party services that you want to use.
* Not tested and not supported on IIS servers.

= Translations =

If you want to make a translation for your language, use the shorten2ping.pot included and (if you want) send me the files to correo@samuelaguilera.com for including it into the plugin package, you'll be credited, of course (NOTE: No sponsored translations allowed).

Credits for present translations:

* Italian translation (it_IT) made by Riccardo Vianello AKA etms51
* Traditional Chinese translation (zh_TW) made by Pseric.
* French translation (fr_FR) made by Olivier.
* Polish translation (pl_PL) made by Darek Skonieczka. 
* Spanish translation (es_ES) made by myself :)
    	
== Installation ==

* Extract the zip file and just drop the contents in the <code>wp-content/plugins/</code> directory of your WordPress installation (or install it directly from your dashboard) and then activate the Plugin from Plugins page.
* After that go to options page 'Shorten2Ping' and fill the required information for your accounts, and customize the message template if you want.
* Now you're ready, the plugin will notify Ping.fm or Twitter (at your choice) everytime you publish a new post (and Ping.fm will do the same to every site that you configured there, if you use this service).
  
== Frequently Asked Questions ==

= What to do when I need support? =

<strong>IMPORTANT!!: At present Seesmic has blocked the API key for this plugin, you can <a href="http://ur1.es/djjSqf">read more here</a>. So I have added support for using email notification, this is working for some users and not for others. Sorry but I can't do it more about this, so blame to Seesmic not me.</strong>

I'm sharing this plugin that I made for personal use to anyone who wants to use for free. I do it in my spare time.

Therefore I'm not giving personal support, if you write an email to me regarding support questions I'll not reply it.

If you need support post a new topic at WordPress.org forums and tag it with <strong>shorten2ping</strong> tag.

I’m subscribed to that tag by RSS, and I check it from time to time trying to help people if the question/problem is not covered by this FAQ, readme, or previous forum posts.

But remember, <strong>this plugin relies on Ping.fm service</strong>, so if Seesmic want they can block you in any way (or do whatever they want to the service behaviour), and they don't give warns to anyone. That is a fact.

So <strong>is not only a matter of the plugin working or not working</strong>. Is about a third party service working (for you) or not working. 

= Will this plugin works in WordPress older than 2.7.x? =

Maybe, but use it at your own risk. I'll not support anyone using outdated WP (or outdated PHP). At the moment of writing this I&#8217;m running this plugin on <strong>WordPress 2.9 and PHP 5.x</strong> and works fine, and was running without problems on <strong>WP 2.8.x and 2.7.x</strong> too. If you run anything below <strong>WP 2.7 and PHP 5.x</strong>, please update for your own good! (and dont ask me for support).

= Why you did this plugin? =

I wanted a <strong>(single) simple</strong> plugin for using Ping.fm + Bit.ly to notify about new posts to my contacts.

= Are you planning to add more features? =

At first only a few little improvements maybe. But if someone suggest a nice feature, and if I have time enough maybe I'll add it.
But it's not my priority. I want to keep it simple.

= I want to show the short permalink to my visitors. How can I do this? =

Simply put <code><?php short_permalink(); ?></code> in your theme where you want to show short permalink. You can add the parameter 'linktext', <code><?php short_permalink('linktext'); ?></code> and it will use the short permalink as text for the link too. Or if you have advanced knowledge of WordPress
theme coding, you can get the <code>'short_url'</code> post meta directly and showing it as you like.

= Hey man!, the same than above question but with Ping.fm =

From sometime ago Ping.fm has his own link shortener service too, so if you disabled Shorten2Ping option to make shorlinks, but you see http://ping.fm/xxxx when you notify a post through Ping.fm, you must disable this service in your Ping.fm account settings.

= Facebook is showing an image from my page header that I dont want to use for that, how can I select wich image to show when sending the post to Facebook? =

Since 1.3 version, Shorten2Ping adds a meta field in the single post view (the one that Facebook will scan) telling Facebook to use the first image <strong>uploaded and inserted</strong> in the post. If you want to override this, or simply you didn't uploaded any image to the post (even if you inserted one), you can add a custom field to the post named 'fb_img' and put the <strong>full</strong> URL to the image in the value for this custom field.

= My post has an image inserted into it, but your plugin is not inserting the Facebook meta to use this image for the thumbnail, what happens? =

It only works with images that you uploaded to <strong>THAT</strong> post, so if you inserted an image from the media library that was uploaded previously to other post. You'll need to use the 'fb_img' custom field described before. I could add some code to sort this out, but the only way to make that (scanning the post content) could make the posting process slower if you use big images.

= I'm trying to use Ping.fm posting email but is not working and no error in post custom fields. What can I do? =

Some users reported this problem and solved after resetting posting email at Ping.fm site and update it in Shorten2Ping settings page.

= Can I use Jetpack wp.me feature (or another wp.me related pluign) while use wp.me in Shorten2Ping too? =

No. You can't. You have two options: Disable wp.me module in Jetpack OR use another shortener in Shorten2Ping config.

If you're using another plugin that manages wp.me links, simply don't use wp.me in Shorten2Ping or deactivate the other plugin.
                                    
== Changelog ==

= 1.4.8 =

* Fixed incompatibility with Stats from Jetpack causing a 'You do not have sufficient permissions to access this page.' error message.
* Added French translation, thanks to Olivier for it.
* Added Polish translation, thanks to Darek Skonieczka for it.


= 1.4.7 =

* Seesmic (owners of Ping.fm) thinks all users of Shorten2Ping are spammers so they decided to supend API key of this app (more info here: http://ur1.es/dlwqTX) so the plugin stopped working some days ago.
* Added option to send updates using posting email (http://ping.fm/email/), so now we don't need a f*cking API key!

= 1.4.6 =

* Removed support to send notifications directly to Twitter (not OAuth support, sorry).
* Removed tr.im support (that shortener is dead).
* Some code cleanup after removed services.

= 1.4.5 =

* Added support for using post tags as hashtags for Twitter, see options page for more information. (Thanks to evardsson for the code).

= 1.4.4 =

* Fixed a little bug in the new bit.ly function.

= 1.4.3 =

* Updated to bit.ly API v3.
* Improved error handling for bit.ly (and j.mp).

= 1.4.2 =

* Updated function to remove 'Get shorlink' button if (WP) stats plugin is active with new names of functions used in the latest stats plugin update. 

= 1.4.1 =

* Added is.gd shortener support.
* Added j.mp shortener support.
* Added wp.me shortener support.
* Added cli.gs shortener support.
* Added Traditional Chinese translation (zh_TW) , thanks to Pseric.
* Updated spanish (es_ES) translation.
* Improved Facebook Thumbnail support. Now uses the new post thumbnail function if available and thumbnail was defined in the post by the user. If not, uses the first attached image or the one the user sets using fb_thumb custom field (like previous version).
* Changed su.pr function to use CURL instead of fopen.
* Changed from rel="short_url" to rel="shortlink". So now uses the same like wp.me
* Improved settings handling using WP API for settings.
* Fixed removing of the 'Get shorlink' button if (WP) stats plugin is active.

= 1.3 =

* Added a function to remove the new wp.me shortlink creation functions present in Wordpress.com stats plugin (if you're using Shorten2Ping you dont need support for wp.me short links).
* Improved Facebook support: Now if you upload and insert an image in your post, Shorten2Ping will add the needed tag in your post code to tell Facebook to take this image for the preview and not the first image in your page's code like used to be before. If you want to force the use of an image, you can add a new custom field to the post named 'fb_img' and put the <strong>full</strong> URL to the image in the value for this custom field.
* Added function to remove HTML tags (if any) from post titles before sending notifications.
* Updated compatibility tag to WordPress 2.9.

= 1.2.8 =

* Finally fixed html entities in title when using Ping.fm to notify new posts (not happened with Twitter). The fix consists in using $post->the_title instead of get_the_title($post_id), so not really a Shorten2Ping's bug but different output for two WP functions that should do the same.
* Improved options page. Now looks better and it's XHTML valid code :)
* Updated locale file (.pot) and es_ES translation to reflect some changes in options page.

= 1.2.4 =

* Added settings link on plugins page
* Fixed bug in Su.pr support (thanks to Brad for reporting it!)

= 1.2.2 =

* Added italian translation made by Riccardo Vianello AKA etms51 
* Improved handling of settings when updating from 1.1.3 to 1.2.x
* Added some code to autofix blank settings created by 1.2 on new installations see http://wordpress.org/support/topic/319359?replies=4 (now you dont need to do that manually, simply deactivate and activate again the plugin).

= 1.2.1 =

* Fixed bug that prevents the plugin options to work on new installations.

= 1.2 =

* Changed checking user level (number based) to checking capabilities for the options page.
* Added YOURLS shortener support.
* Added Su.pr shortener support. (User requested feature).
* Added 'linktext' parameter to short_permalink() theme tag. Now you can choose between using short link as text for the link or use the "Short URL" text (default behaviour). (User requested feature).
* Added 'Self domain' option for shortened permalinks. If your domain is short enough for you, this option will not use any shortener service, but instead will use the post ID (default WP permalinks).

= 1.1.3 =

* Added checking to avoid to ping new pages. Now only posts are notified (as intended from start of making this plugin).

= 1.1.2 =
* Removed adding and checking of post meta data 'pinged = yes'. That was not needed since changes on 1.1.1
* Added 'both' option by user request to make possible to send notifications to both services (Ping.fm and Twitter) at once.
* Fixed typo that may cause users with no admin level to access to the options page. (Thanks to David Jack Wange Olrik for reporting the issue.)

= 1.1.1 =

* Changed action hook. Now the ping function is called only when post changed status from X to publish (where X can be new, draft, pending or future). So now, if you edit an old post (that you published before installing Shorten2Ping) or the post has any else status than mentioned this plugin does nothing.
* Removed echo statement at tr.im function (used while debugging) that causes no returning to post edit page after publishing on some cases.
* Removed @ operator at json_decode functions, now if any error happens while calling json_decode it will show on screen.

= 1.1 =

* Added support for http://twitter.com and http://tr.im
* Some other minor improvements/cleanup in the code.
* Store settings in an array to reduce calls to database.
* Added options for choose shorten and notification services, and to turn off them (so you can use Shorten2Ping only for notification if your domain is already short enough for you, or use Shorten2Ping only to get shortened urls for your posts).

= 1.0.2 =

* Replaced PHPingFM by Dmitri Gaskin for a single function based on the one by Sold Out Activist for the pingPressFM.

= 1.0.1 =

* Fixed a typo and Ping.fm developer approved.

= 1.0 =

* Initial release.

Originally based on WordTwit 1.2 by Duane Storey.

PingFM function based on one by Sold Out Activistclass for the pingPressFM plugin, and Bit.ly function by David Walsh & Jason Lengstorf.
