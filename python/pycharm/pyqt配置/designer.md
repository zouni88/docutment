### pycharm 配置pyqt 可拖拽控件工具


1. 打开`pycharm` 找到`Tools/External_Tools` 新增一个
![external](res/external_tools.png)
2. 找到`desiginer.exe`位置,我的是在anaconda3安装的，就在我的虚拟环境目录下面找到：

    D:\Anaconda3\envs\python_basic\Scripts\designer.exe

`Working directory` 这个路径是工作路径，所以一般就填入`$FileDir$`

![QtDesigner](res/QtDesigner.png)

3. 编辑完UI后，还需要转换成`py`文件才行，所以需要配置pyui转换

![pyui](res/pyui.png)

4. 第一次使用,先新建一个ui文件先

  ![desiginer_2](res/designer_2.png)

  ![qtdesigner_1](res/qtdesigner_1.png)
  妥妥拽拽一些控件华丽界面就完成了

5.  最后一步，转换成`py`文件
  ![designer_3](res/designer_3.png)

6. end
