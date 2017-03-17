유피넬 서버 안내페이지
========
서버별 안내 페이지입니다.
```shell
git clone https://github.com/upnl/greeting.git

# apache2
sudo mv greetings /var/www/
# nginx
sudo mv greetings /usr/share/nginx/
```

### 웹서버 설정
```apache
# apache2
<VirtualHost *:80>
  DocumentRoot /var/www/greeting/<SERVER_NAME>
</VirtualHost>
```
```Nginx
# nginx
server {
  listen 80 default_server;
  server_name _;
  root /usr/share/nginx/greeting/<SERVER_NAME>;
}
```
