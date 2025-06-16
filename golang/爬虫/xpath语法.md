当涉及到网页抓取和解析HTML/XML文档时，XPath是一种强大的定位和提取数据的工具。XPath（XML Path Language）是一种在XML文档中定位节点的语言。下面是一些关于XPath的详细解释和案例：
基本介绍
1. XPath基础
XPath的基本语法如下：
```
/         # 从根节点开始
//        # 选择匹配的任何位置
.         # 当前节点
..        # 父节点
@         # 选择属性
[node]    # 选取所有node子元素
[@attr]   # 选取带有attr属性的所有元素
```
2. 选取节点
使用XPath选取节点，例如：
```
//div          # 选择所有div元素
//div[@class]  # 选择带有class属性的div元素
//div[@id='myId']  # 选择id属性为'myId'的div元素
```
3. 路径表达式
XPath使用路径表达式来选取节点。例如：
```
//div/p   # 选择所有div下的p元素
//div//p  # 选择所有div下的所有p元素
```
4. 谓词
XPath中的谓词用于过滤节点。例如：
```
//div[@class='highlight']  # 选择class属性为'highlight'的div元素
//ul/li[position()<3]      # 选择ul下的前两个li元素
```

5. 通配符
使用通配符匹配元素，例如：
```
    //*        # 选择所有元素
    //div/*    # 选择所有div下的所有子元素
```
6. 文本提取
使用XPath提取文本内容，例如：

```
//p/text()   # 提取p元素的文本内容
```
