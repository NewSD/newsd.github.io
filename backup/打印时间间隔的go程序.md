```go


package main

import (
	"fmt"
	"time"
)

// 定义一个表示时间间隔的结构体
type Duration struct {
	time.Duration
}

// 实现一个将时间间隔格式化为字符串的方法
// String 方法将 Duration 类型的值转换为字符串格式，精确到秒的小数点后两位。
// 这个方法使得 Duration 类型的值可以以更加直观的方式进行显示。
func (d Duration) String() string {
	// 使用 fmt.Sprintf 将 Duration 的秒数转换为字符串格式，保留两位小数。
	return fmt.Sprintf("%.2f seconds", d.Seconds())
}

// main函数是程序的入口点
func main() {
	// 初始化一个Duration结构体实例，表示2秒333毫秒的时间间隔
	// 创建一个时间间隔的实例
	duration := Duration{Duration: 2*time.Second + 333*time.Millisecond}

	// 输出duration的值
	// 打印格式化后的时间间隔
	fmt.Println(duration)
}


```