# lyp_homework-cli
//// 用于存放step01的homework-cli, 以下是homework具体内容：

1.找到在 Ubuntu 系统中可以用于计算文件内容 MD5 值的命令
answer：
   1）计算文件的MD5值：md5sum 文件全路径名
   2）计算字符串的MD5值：echo -n '被选字符串' | md5sum
   
2.找到在 Ubuntu 系统中可以用于比较两个文件的内容的差异的命令
   1）cmp file1 file2             //逐字节比较，在第一处不同退出并显示该处不同
   2）comm file1 file2            //逐行比较，输出两文件相同的行
   3）diff                        //逐行比较，输出差异行
   4）uniq                        //报告或省略重复的行
