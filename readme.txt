=== SO Pinyin Slugs ===
Contributor: senlin
Tags: pinyin, permalinks, slugs, Mandarin, Chinese
Requires at least: 3.5.2
Tested up to: 3.6
Stable tag: 0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Transforms Chinese character titles (of Posts, Pages and all other content types that use slugs) into a permalink friendly slug, showing pinyin that can be read by humans and (Chinese) search engines alike.

== Description ==

The SO Pinyin Slugs plugin is a fork of the original [Pinyin Permalinks](http://wordpress.org/plugins/pinyin-permalink/) plugin by user [xiaole_tao](http://profiles.wordpress.org/xiaole_tao/) who has seemingly abandoned his plugin as he never responded to emails.

The original plugin can basically only be used on Chinese only websites; as soon as you install it on a bi/multilingual site it messes up the slugs of the non-Chinese languages.

This fork has been adapted by my ex-colleague [Denis Cao](caoyongsheng@gmail.com) in such a way that the slugs of the non-Chinese language remain untouched and only the Chinese character slugs will be transformed into pinyin.

Chinese characters don't come out good in permalinks. Without the SO Pinyin Slugs plugin activated, the example post I made for the screenshot will get a slug like this: *%e6%90%9c%e7%b4%a2%e5%bc%95%e6%93%8e%e4%bc%98%e5%8c%96*. With the plugin the slug automatically becomes *sousuoyinqingyouhua*. 

Search engines such as [Baidu](http://www.baidu.com) obviously cannot make much of the first slug, but they can handle pinyin perfectly, especially when it is written as one long string without hyphens or underscores

Pinyin slugs are best read by search engines such as [Baidu](http://baidu.com) as one long word, so instead of transforming "中国" into two separate words divided by a hyphen or an underscore (the original plugin has this as options), it is best transformed into "zhongguo". The only option SO Pinyin Slugs therefore has left is the length that you can limit to an x amount of letters. The default is 100, which should be plenty for most.

I have decided to only support this plugin through [Github](https://github.com/senlin/so-pinyin-slugs/issues). Therefore, if you have any questions, need help and/or want to make a feature request, please open an issue over at Github. You can also browse through open and closed issues to find what you are looking for and perhaps even help others.

**PLEASE DO NOT POST YOUR ISSUES VIA THE WORDPRESS FORUMS**

Thanks for your understanding and cooperation.


== Installation ==

= Wordpress =

Quick installation: [Install now](http://coveredwebservices.com/wp-plugin-install/?plugin=so-pinyin-slugs) !

 &hellip; OR &hellip;

Search for "SO Pinyin Slugs" and install with the **Plugins > Add New** back-end page.

 &hellip; OR &hellip;

Follow these steps:

1. Download zip file.
2. Upload the zip file via the Plugins > Add New > Upload page &hellip; OR &hellip; unpack and upload with your favorite FTP client to the /plugins/ folder.
3. Activate the plugin on the Plug-ins page.

Done!


== Frequently Asked Questions ==

= Known Issues: =

* SO Pinyin Slugs will not transform existing slugs
* If the title contains both Chinese characters and alphanumeric characters (abc, 123, etc.) SO Pinyin Slugs will ignore the latter. So if these alphanumeric characters are important, you will need to add them manually to your slug.

= Can I use this plugin also for Traditional Chinese? =

No, the dictionary part of the plugin only contains Simplified Chinese. If you want, you can check what words the dictionary contains by going into `inc/functions.php`

= I have an issue with this plugin, where can I get support? =

Please open an issue over at [Github](https://github.com/senlin/so-pinyin-slugs/issues), as **I will not use the support forums** here on WordPress.org

== Screenshots ==

1. Settings page
2. New Post with title in Chinese characters and auto-generated pinyin slug; Baidu Search Results page underneath

== Changelog ==

= 0.1 =
* First stable release