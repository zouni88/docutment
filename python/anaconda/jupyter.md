生成配置文件
```
jupyter notebook --generate-config
```
生成密钥
```
jupyter notebook password
# 设置密码：123456

```

```Shell
# 如下地址
```Shell
/root/.jupyter/jupyter_notebook_config.json
```
# 密钥：
sha1:23524a335a85:461a1f37e8e32af1ab8899329b3e41c41ea6e546

```

![jupyter](res/jupyter_1.png)


### 修改配置文件
```
vi /root/.jupyter/jupyter_notebook_config.py
```
修改如下内容：
```Shell
# 允许 作为root访问
c.NotebookApp.allow_root = True
# 允许所有地址访问
c.NotebookApp.ip='*'   
# 密钥：/root/.jupyter/jupyter_notebook_config.json 文件的内容
c.NotebookApp.password = u'sha1:03...

```
