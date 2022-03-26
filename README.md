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

3.实现一个名为 odd-or-even 的 Bash function，可以用来判断给其提供的第一个参数是奇数还是偶数，奇数时输出 odd，偶数时输出 even

function odd-or-even2(){
  n=$1
  n1=$(echo $n | grep -c "[^0-9]")
  if [$n1 -eq 1]
  then
       echo "你输入的不是数字！"
       exit 1
  fi

  n2=$[$n%2]
  if [$n2 -eq 0]
  then
       echo even
  else
       echo odd
  fi

}

4.实现一个名为 next 的脚本，当在 CLI 里执行 $ next （$为提示符，不需要输入）时就返回一个整数，第一次返回 1，每执行一次加 1

5.一个文件含有 N 行内容，每行的内容都是一个大于等于 0 的整数，无任何空行或其它内容，使用 one-liner 的形式对该文件中的数字求和

6.top10
![image](https://user-images.githubusercontent.com/101808060/160234159-de071388-a6d7-46f9-91df-8def63308daf.png)
