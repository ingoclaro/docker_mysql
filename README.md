Docker image for mysql

Based on the stock [mysql image](https://registry.hub.docker.com/_/mysql/) I added the following env variables:

MYSQL_DATA_DIR=/var/lib/mysql

Where to store the mysql data. Since the default is a volume it's not preserved if you want to save the container as a new image. With this env variable you can change the directory.
