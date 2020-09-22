docker run --restart=unless-stopped --name nextcloud -d -p 8080:80  -v /var/www/mynextcloud/config:/var/www/html/config -v /var/www/mynextcloud/data:/var/www/html/data mynextcloud
