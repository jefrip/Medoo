Medoo
=====

The Lightest PHP database framework to accelerate development

Main Features
----------------
### Lightweight ###
Only 8KB, one file included.

### Easy ###
Extremely easy to learn and use, friendly construction.

### Powerful ###
Support various common SQL queries.

### Compatible ###
Support various SQL database, including MySQL, MSSQL, SQLite and more.

### Security ###
Prevent SQL injection.

### Free ###
Under MIT license, you can use it anywhere if you want.

Get Started
-------------
```
// Include Medoo
require_once 'medoo.php';

$config = array(
	'type' => 'mysql',
	'name' => 'mydb',
	'server' => 'localhost',
	'username' => 'username',
	'password' => 'password'
);

//optional
$options = array(
    PDO::ATTR_PERSISTENT => true //if using persistent connection
);

// Initialize
$database = new medoo($config, $options);


// Enjoy
$database->insert('account', [
	'user_name' => 'foo'
	'email' => 'foo@bar.com',
	'age' => 25,
	'lang' => ['en', 'fr', 'jp', 'cn']
]);
```
Links
------
Official website: [http://medoo.in](http://medoo.in)

Documentation: [http://medoo.in/doc](http://medoo.in/doc)