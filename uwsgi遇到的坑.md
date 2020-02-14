### 编译配套 ssl的 uwsgi

#### 安装编译需要的环境
```
yum install openssl
yum install openssl-devel
```
#### 安装 greenlet
```
pip3 install greenlet
```

CFLAGS="-I$/usr/bin/python3.6" UWSGI_PROFILE="asyncio" pip install uwsgi --no-use-wheel

