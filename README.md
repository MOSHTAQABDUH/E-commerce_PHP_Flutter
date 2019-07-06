# fastapp

This project is an E-commerce mobile app, written in Flutter and PHP. MySQL is used as the database.

The following steps will show you how to run the app (in Windows):
_1. Install [Flutter](https://flutter.dev/docs/get-started/install) and [XAMPP](https://www.apachefriends.org/download.html).
_2. Clone this repository or download it as a .zip file.
_3. Move flutter_server folder in flutter_server/flutter_server (as you see in this repository) to htdocs in your XAMPP directory (usually in C:\xampp). This folder contains .php files for the server and uploadImage folder for products' images storage.
_4. Run XAMPP, click to **Start** and **Admin** buttons in 2 modules Apache and MySQL. Now we create the database, table and user for the app. 

**Create database**

__4.1. At http://localhost/phpmyadmin/, click **New** to create a new database.

__4.2. Set a name for the database (e.g. flutter_php_db).

**Create table**

__4.3. In **Create table** area, set a name for a table (e.g. userinfo) and click **Go** button => a table has been created (which represents an entity).

__4.4. Add some rows for the table (Each row represents an attribute of the entity). The first row should be **id** and should be the primary key of the table (tick **A_I** checkbox to set it as the primary key and activate AUTO_INCREMENT). Set the [data type](https://www.w3schools.com/sql/sql_datatypes.asp) of each row. 

(follow 4.3 and 4.4 to create 6 tables: 
Table 1: userinfo(id int, name varchar(30), account text, password text, email text, phone text, type varchar(6), company text) with id, name, account, password, email, phone, type and company are the names of the rows and int, varchar, text are the data types of each row.

Table 2-6: dogiadung, giaydep, quanao, smartphone and xabong (respectively mean "furniture", "shoes", "clothes", "smartphone" and "shampoo" in English). Each table has 6 rows: id int, name text, image text, description text, price text, producer text.)

**Create user**

__4.5. Click **Home** button under phpMyAdmin icon, choose **User accounts** tag.

__4.6. Click **Add user account**.

__4.7. Set username (e.g. flutterphp), host name (it should be localhost) and password (it's optional).

__4.8. User account overview -> Edit privileges. Tick SELECT, INSERT, UPDATE and DELETE.

__4.9. In **Database** tag, choose the name of the database (in 3.2).

_5. In .dart files, change the IP address to your IP address (cmd -> ipconfig).
_6. Connect your smartphone to your PC and execute the code.
_7. Enjoy.
