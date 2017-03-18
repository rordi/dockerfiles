PHP-FPM Dockerfile for CakePHP Apps
-----------------------------------

A Dockerfile to create an images suitable to run a CakePHP 3.x applicatino. 

The image runs a PHP-FPM process on port 9000. The image comes with a mysql
client to connect to a MySQL server running in another container. Additionally,
the pdo_mysql, mcrypt, gd and intl PHP extensions are enabled.

Use the image in conjunction with an Nginx or Apache image.
