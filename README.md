# fop-pickr

Step1: Create a data container for MySQL
docker create --name mysql-pickr-data tonym2105/mysql-data-container
* You can create your own MySQL data container image.

Step 2: Start the MySQL container
docker run --volumes-from mysql-pickr-data --name pickr-mysql -e MYSQL_USER=mysql -e MYSQL_PASSWORD=mysql -e MYSQL_DATABASE=pickr -e MYSQL_ROOT_PASSWORD=supersecret -d mysql



Shout Outs!

* Running MySQL with Docker
http://blog.arungupta.me/docker-mysql-persistence/

