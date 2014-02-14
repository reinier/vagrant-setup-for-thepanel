# Read me

## How to use this?

This [Vagrant](http://www.vagrantup.com) setup is created for [The Panel](http://thepanel.io). Just put these files and directories (except for this readme.md) in the root of your The Panel project and use vagrant up to provision your server. This setup is for *development* only.

Add the following configuration variables to The Panel into the right place:

### app/config/app.php

	'url' => 'http://thepanel.dev',

### app/config/bookmarklet.php

	'base_url' => 'thepanel.dev',

### app/config/database.php

	'driver'    => 'mysql',
	'host'      => 'localhost',
	'database'  => 'thepanel_db',
	'username'  => 'thepanel',
	'password'  => '123abc',

## Use vagrant just as you think you would

	> vagrant up

etc.

## Domain

The Panel will be running on [http://thepanel.dev](http://thepanel.dev) when you add this to your host file (`/etc/hosts` on Mac):
	
	192.168.56.101 thepanel.dev