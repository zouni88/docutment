```
docker run -itd --name=nginx -p 80:80 -p 443:443 -v /usr/local/small/nginx/conf.d:/etc/nginx/conf.d -v /usr/local/small/web/facepark/static:/root/web/facepark/static nginx:2.0
```
