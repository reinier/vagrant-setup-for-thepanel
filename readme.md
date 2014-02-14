# Read me

## How to use this?

This vagrant setup is created for The Panel. Just put these files and directories (except for this readme.md) in the root of your The Panel project.

Add the following configuration variables into the right place place:

### app/config/app.php
'url' => 'http://thepanel.dev',

### app/config/bookmarklet.php
'base_url' => 'thepanel.dev',

### app/config/database.php
driver'    => 'mysql',
'host'      => 'localhost',
'database'  => 'thepanel_db',
'username'  => 'thepanel',
'password'  => '123abc',

## Use vagrant just as you think you would

	> vagrant up