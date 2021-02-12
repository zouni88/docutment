# flutter web 开发
1. 开启`web`支持

    > flutter config --enable-web

2. 再次 执行
    > flutter doctor

3. 一切正常之后,正常创建项目，会多出一个`web`文件夹  

    以前旧的项目可以执行以下命令：
    > flutter create .

4. 运行在浏览器看下效果：
    >flutter run -d edge

    我这里用的 microsoft edge 浏览器
5. 打包
    > flutter build web

    > flutter build web --release  //生产环境打包
    
    可以看到 `build` 目录下多出一个**web** 文件夹 