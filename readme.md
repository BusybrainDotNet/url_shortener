# URL Shortner System
URL Shortner API System 

### Changelog

#### V 1.0.0
Initial Release

### Author
[Oluniyi Benjamin] (www.linkedin.com/in/oluniyi-benjamin-o-a654bb155)

### License

URL Shortner System is licensed under The MIT License (MIT). Which means that you can use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the final products. But you always need to state that Oluniyi Benjamin is the original author of this API system.


### API Test

- [Test Suite of this project can be found via this link. All Test Case Images Are Saved In The Same Folder](http://127.0.0.1:8080/Test Suite/)

### info on running the API

- [The local development server used for this project is laragon. feel free to use WAMP/XAMMP etc] (https://wwww.laragon.org)

- [Navigate to the directory where you have located this PHP project, sstart the terminal or cli](cd php-project-name)

- [Once you are in the project folder then run the following command to start the PHP app.](php -S 127.0.0.1:8080)

- [Following output will be displayed on your terminal screen.](PHP 7.2.19 Development Server started at Thu Jul 25 14:33:53 2021
Listening on http://127.0.0.1:8080
Document root is E:\laragon\www\url-shortner
Press Ctrl-C to quit.)

- [Check your project on the following url:](http://127.0.0.1:8080)

- [Access the database root user via command-line to create the database.](mysql -u root -p)

- [Create a new MySQL database.](CREATE DATABASE url;)

- [Check the database.](SHOW DATABASES;

+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| url           |
| sys                |
+--------------------+)

- [Use the database.](use url;)

- [Once you are done with the database creation, then you should run the SQL script to create the table.](CREATE TABLE `url_info` (   
`long_url` VARCHAR(200) NULL DEFAULT NULL ,  
`short_url` VARCHAR(200) NULL DEFAULT NULL ,
`created` DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP ,    
PRIMARY KEY  (`short_url`)
) ENGINE = InnoDB   DEFAULT CHARSET=latin1 ;)

- [Make sure what table you have created.](SHOW tables;

+--------------------+
| Tables_in_url |
+--------------------+
| url_info           |
+--------------------+)

- [The statistics folder shows the details of the short link entered.](http://127.0.0.1:8080/statistics/(__SHORT_URL__))

- [Proceed to use any API Test tool, POSTMAN was used in the development stage.](www.postman.com)


### API End Points

- [Encode Long URL and populate DB](http://127.0.0.1:8080/api/encodes.php)

- [Decode short url and return Long](http://127.0.0.1:8080/api/decodes.php)

- [URL statistics](http://127.0.0.1:8080/api/statistics.php)


### End
