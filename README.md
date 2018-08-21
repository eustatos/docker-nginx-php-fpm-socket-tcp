For run containers fork this repository and execute:
```bash
git clone http://github.com/<you_github_username>/docker-nginx-php-fpm-socket-tcp.git
cd docker-nginx-php-fpm-socket-tcp
docker-compose up -d
```
Navigate in your browser `http://localhost:8880/test.php`. You must see `phpinfo()` output.
Now containers connected via socket.
Apache banchmark for this in `data\socket.log`

For use tcp connection
```bash
docker-compose stop
git checkout -f tcp
docker-compose up -d --build
```

Reload your page `http://localhost:8880`.
Now containers connected via tcp.

Apache banchmark for this in `data\tcp.log`


