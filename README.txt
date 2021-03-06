===========================================================================
| This version is an effort to provide up-to date version of Rockmongo by |
| including latest patches from a number of forks found on Github.        |
===========================================================================

Introduction
--------------------------------------
RockMongo is a MongoDB administration tool, written in PHP 7, very easy to install and use.
This tool can be used with MongoBD 2.4 to Mongo 3.4


Installation
--------------------------------------
1. Install PHP runtime environment if you don't have one yet, such like Apache Httpd, Nginx ...
2. Install MongoDB PHP driver (http://us.php.net/manual/en/mongodb.installation.php)
3. Run "git clone https://github.com/IngenierosWeb/rockmongo.git"
4. Copy config-sample.php to config.php
5. Open the config.php with your convenient editor, change host, port, admins and so on to yours
6. Install comproser (https://getcomposer.org/doc/00-intro.md)
7. Run "composer install"
8. Visit the index.php in your browser, for example: http://localhost/rockmongo/index.php
9. Login with admin username and password, which is set "admin" and "admin" as default
10. Play with your MongoDBs!


Upgrade from old version
--------------------------------------
1.Copy all files excluding config.php to your old version directory
2.Done!

Use for MongoDb 3 or higher
--------------------------------------
$MONGO["servers"][$i]["mongo_auth"] = true;
$MONGO["servers"][$i]["mongo_db"] = false; //required if you use not root user
$MONGO["servers"][$i]["mongo_user"] = "root";
$MONGO["servers"][$i]["mongo_pass"] = "root password";
$MONGO["servers"][$i]["mongo_version"] = "3.4";


Contributors
--------------------------------------
iwind.liu <iwind.liu@gmail.com> Leader
leblanc.simon <leblanc.simon@gmail.com> French translation
Klaus Silveira <klaussilveira@gmail.com> Brazilian translation
bmansion <bmansion@mamasam.net> Some small changes
Vladimir Razuvaev <vladimir.razuvaev@gmail.com> Implement features.
Anton Zering <anton.zering@gmail.com> German translation
Borda Juan Ignacio <juanignacioborda@gmail.com> Panels Layout
Diego Baravalle <diegobaravalle@gmail.com> Spanish Translation


Thanks
--------------------------------------
* Many thanks to led24.de for cute icons.
* Thank Michal Migurski(<mike-json@teczno.com>) for perfect Services_JSON class.
* Thank OFC,  we borrowed json_format() function to make JSON pretty.
* Thank jQuery, a popular javascript library.
* Thank snipplr.com for mime types mapping.
* Also thank these guys (Marcin, Tyler, Richard, Idan, ...) who spent their time on
  sending feedbacks and advices to me, and let me know i am not alone.
* Thank Klaus Silveira for Brazilian translation
* Thank leblanc.simon for French translation

Bugs & Issues
--------------------------------------
Please feel free to report any bugs and issues to https://github.com/IngenierosWeb/rockmongo/issues


Contributing
--------------------------------------
Somebody who want to contribute to the project, may help us by doing these:
* Translate messages from English to other languages (you can see them in app/langs directory)
* Request a pull with fixed code or new functionallities