### 空字符串
```golang
type Person struct{
    Name string
    Age int `json:"age"`
}
func main(){
    p := Person{Name:"cao",Age:12}
    resbyte,err := json.Marshall(p)
    if err != nil{
      log.Fatal(err)
    }
    resstring := string(resbyte)
    fmt.Println(resstring)
}
`json:"age,oemiempty"` : golang语法规定 结构体字段必须大写 开头， json生成字符串 是小写开头， 声明一个小写字母 开头 的名称
oemiempty ： 值为空，就忽略此字段
```
