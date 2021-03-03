# go run test 不打印 详情
> go test -v # 正常命令应该是这样的，vscode 默认运行 不带-v
修改工作空间设置
```json
{
    "go.inferGopath": false,
    "go.testFlags": ["-v"],  //增加这一行
}
```
再运行就正常了。

