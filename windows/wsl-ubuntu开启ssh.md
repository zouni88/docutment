clion配置toolschains:
1. mingw64
2. wsl - ubuntu  
    1. 打开终端 
    2. 进入subsystem,安装ssh
        ```shell
        small@small:~$ sudo apt-get install openssh-server
        [sudo] password for small:
        Reading package lists... Done
        Building dependency tree
        Reading state information... Done
        openssh-server is already the newest version (1:8.2p1-4ubuntu0.2).
        0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
        ```
    3. 编辑ssh配置文件：
        ```shell
        small@small:/etc/ssh$ sudo systemctl enable ssh
        # 解开以下注释
        Port 2222
        AddressFamily any
        ListenAddress 0.0.0.0
        ListenAddress ::

        # 还有这里
        # To disable tunneled clear text passwords, change to no here!
        PasswordAuthentication yes
        ```
    4. 启动ssh
        ```shell
        small@small:/etc/ssh$ sudo service ssh restart
        * Restarting OpenBSD Secure Shell server sshd
        ```
    5. clion 测试链接就 ok了！