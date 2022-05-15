
To do that I added another table inside database (exported in the file if this SQL
have errors) and I used phpMyAdmin.
And I'm using port 2222 on localhost, so maybe that will be case.

POSTS: 
CREATE TABLE `students`.`posts` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `usr_id` INT NOT NULL,
  `title` VARCHAR(255) NOT NULL,
  `body` TEXT(1000) NOT NULL,
  `created_at` DATATIME NOT NULL,
  PRIMARY KEY (`id`));

USERS:
CREATE TABLE `students`.`users` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `username` VARCHAR(200) NOT NULL,
  `email` VARCHAR(255) NOT NULL,
  `password` VARCHAR(255) NOT NULL,
  PRIMARY KEY (`id`));
