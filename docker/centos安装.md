### Step 1: 安装必要的一些系统工具
```Shell
sudo yum install -y yum-utils device-mapper-persistent-data lvm2
```
### Step 2: 添加软件源信息
```Shell
sudo yum-config-manager --add-repo https://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo
```
### Step 3: 更新并安装Docker-CE
```shell
sudo yum makecache fast
sudo yum -y install docker-ce
```
### Step 4: 开启Docker服务
```shell
sudo service docker start
```
