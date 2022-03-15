## 添加其他仓库到当前仓库
    
    git submodule add https://github.com/alex-shpak/hugo-book themes/book
 - 添加完成项目根目录下会多出一个 `.gitmodules` 文件
 
## 同步其他仓库更新
    //一步到位，不用挨个查找，直接遍历一遍
    git submodule foreach git pull

## 删除submodule

    git submodule deinit themes/book