# go-lib-test

## 笔记

go.mod 中名字需要和仓库地址一样

`github.com/Mark24Code/go-lib-test`

整个的逻辑就是围绕目录，或者网络 url 进行

包的库不需要提供 main.go 只需要提供文件夹，具体代码。

可以打 版本号  比如  v0.0.1 那么 下载使用 go get 也要使用这个 版本号

引入使用

`go get github.com/Mark24Code/go-lib-test@v0.0.1`

在 代码中使用，引用到具体的文件夹即可（默认一个文件夹下所有文件都是一个 package）

```go
import "github.com/Mark24Code/go-lib-test/utils"
func main() {
	println(utils.Add(100,200))
}
```
