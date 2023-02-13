IPBAuthLogin
============

IPBAuthLogin is a plugin for MediaWiki 1.35 and up which integrates MediaWiki with an [Invision Power Board and Invision Community](https://invisioncommunity.com) forum's user database. By enabling the extension, it is possible to log into the MediaWiki installation using IPB user accounts. The extension creates local user accounts on MediaWiki, which are always authenticated though this extension.

As IPB usernames are not case sensitive, extension converts any username into a canonical form, to avoid duplicate local accounts being created for the same user.

Requirements
------------

* MediaWiki 1.35+
* Invision Power Board 3.x | IPS Community 4.x
* MySQL/MariaDB
* PHP 7.0+ (PHP <=5.6: untested & PHP 8.0: tested)
* MySQLi PHP extension

Documentation
-------------

Extensive documentation for the extension can be found on its [MediaWiki extension page](https://www.mediawiki.org/wiki/Extension:IPBAuthLogin).

Installation
------------

This extension can be installed in either of two ways now:

Manual install: Download the tarball from the [MediaWiki extension page](https://www.mediawiki.org/wiki/Extension:IPBAuthLogin).

Using [Composer](https://getcomposer.org/): This extension can now utilize [MediaWiki's built-in support for Composer](https://www.mediawiki.org/wiki/Composer). From the root directory of the MediaWiki installation, create or modify "composer.local.json" with the appropriate variant of following content:
```
{
	"require": {
                  "mediawiki/ipb-auth-login": "~1.0.3"
        }
}
```
Using either method, enable the extension according to the instructions provided on the MediaWiki extension page. 

License
-------

This extension is licensed under the included GPLv3 license.

Contributing
------------

Contributions can be made to the plugin by submitting pull requests through its [GitHub repository](https://github.com/peerau/IPBAuthLogin).

TODO
----

* Support for account recovery through MediaWiki.
* Possible support for account creation through MediaWiki.
