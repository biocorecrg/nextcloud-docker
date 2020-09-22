docker build -t mymysql .

docker run --restart=unless-stopped --name db -p 3306:3306 -e MYSQL_ROOT_PASSWORD=myrootpwd -v /home/admin/mysql:/var/lib/mysql -d mymysql

