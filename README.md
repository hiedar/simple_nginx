# Simple nginx with docker

1. ```export WORKINGDIR=`pwd````
2. ```docker build -t simple/nginx ./nginx```
3. ```docker run -p 8080:80 --name simple_nginx -v $WORKINGDIR/nginx/conf/:/etc/nginx/ -v $WORKINGDIR/nginx/html:/var/www -v $WORKINGDIR/nginx/log:/var/log/nginx -d simple/nginx```

# Thanks
* [Dockerでつくる開発環境【nginxコンテナ編】 | フリップフラップ](http://blog.flup.jp/2016/02/12/devenv_nginx_with_docker/)
