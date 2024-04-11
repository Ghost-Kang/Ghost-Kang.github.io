cut命令：从一个文本文件或者文本流中提取文本列

cut -b list -[n] [file ...]
cut -c list [file ....]
cut -f list [-d delimiter] [-s] [file ...]

-b -c -f 分布表示 字节，字符，字段（byte， character， field）
list表示操作的范围， -你表示具体数字
file表示操作文件名字
delimiter 表示分隔符，默认情况下为TAB；
-s表示不包含哪些不含分隔符的行（有利于去掉注释和标题）
范围表示方法：N 只有第N项， N-从第N一直到行尾； N-M从N项到M项  -M 从第一个行开始到第M项  - 从1行开始到结束的所有项

例子：

1. grep '[[:digit:]]:' /proc/interrupts | cut -c 1-15


2. grep '[[:digit:]]:' /proc/interrupts | cut -c 1-4, 34-


3. cut -f1 -d ':' /etc/passwd | head -15   //  cut -d ":" -f1  /etc/passwd | head -15



