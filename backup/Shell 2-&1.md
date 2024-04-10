linux系统下文件描述符（file descriptor）表示数据流
0：stdin 标准输入
1：stdout 标准输出
2: stderr 标准错误输出
3：other file

>是重定向符号
&类似引用地址的意思

>&是一个整体，不可以分开，分开就没有上述的意思

2>&1 的意思是：将标准错误的信息，发送到标准的输出中

标准输入  0     <或 << 或 <<<     /dev/stdin -> /proc/self/fd/0 -> /dev/pts/0
标准输出 1     >，>>, 1>或 1>>  /dev/stdout -> /proc/self/fd/1 -> /dev/pts/0
标准错误  2   2> 或 2>>      /dev/stderr -> /proc/self/fd/2 -> /dev/pts/0

标准输出：
go run my.go > twz.log
gor urn my.go 1> twz.log
错误输出：
go run my.go  2>twz.log

标准和错误一起输出到文件
go run my.go >twz.log 2>&1
go run my.go &>twz.log


