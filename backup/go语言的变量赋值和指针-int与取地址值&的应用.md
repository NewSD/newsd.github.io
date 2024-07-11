```go
package main

import "fmt"

// main函数是程序的入口点
func main() {
	// 初始化一个整型变量num并赋值为10
	var num int = 10
	// 输出变量num的值
	fmt.Println("num = ", num)

	// 初始化一个指向整型的指针变量p，并将其指向num
	var p *int = &num
	// 输出指针变量p的值
	fmt.Println("p = ", p)
	// 输出指针p所指向的值
	fmt.Println("*p = ", *p)

	// 输出变量num的地址
	fmt.Println("&num = ", &num)
	// 输出指针变量p的地址
	fmt.Println("&p = ", &p)
}


```