---
layout: post
title: ubuntu 升级
---
#分区的时候至少分3个：/，swap和/home，重装的时候，格式化/就可以了，保留/home不要格式化。







一、备份数据。参考：http://ubuntuabc.com/123/?p=92
虽然虽然这样重装理论上不会破坏你的文件，但有时候一些意外的情况（比如误操作或系统有bug）会导致数据丢失。所以还是强烈建议你备份你的重要文件。

二、删除旧的配置文件

因为我不想保留旧的系统设置和软件设置，想安装一个全新的系统，所以要删除旧的配置文件，如果你想保留以前的设置的话，就省略此步骤。

删除配置文件的方法是：
1、用光盘启动系统，进入Live CD。
2、在终端里执行命令“sudo nautilus”，以管理员身份打开文件浏览器。
3、按“Ctrl+H”键显示隐藏文件。
4、删除硬盘/home分区里的“lost+found”和“.Trash-0”文件夹。
5、删除“username”文件夹里所有以“.”开头的文件夹及文件。（“username”是你的用户名）

三、重装系统

前面几个步骤和常规安装一样，这里就不多说了。

重点在“预备硬盘空间”，也就是分区这步。选择“手动指定分区（高级）”。



 

根据分区大小判断，“/dev/sda1”是原来的“/”分区。选择“/dev/sda1”，点“更改...”按钮。



 

不要改变原来的分区容量；在“用于”右边的下拉列表选择分区格式“Ext4日志文件系统”；选中“格式化此分区”；“挂载点”选“/”；然后点“确定”。



 

“/dev/sda5”是原来的swap分区。选择“/dev/sda5”，点“更改...”按钮。



 

不要改变原来的分区容量；选择用于“交换空间”。格式化和挂载点不用选。



 

“/dev/sda6”是原来的“/home”分区。选择“/dev/sda6”，点“更改...”按钮。



 

不要改变原来的分区容量；原来是什么文件系统，现在还是选什么文件系统！不要选择“格式化此分区”！挂载点选择“/home”。



 

检查一下，注意看“/home”后面没有勾选格式化，使用的文件系统（类型）也跟原来一样。然后点“前进”。



 

后面的步骤也是跟常规安装一样，按屏幕提示操作即可。要注意的地方是：
填写身份时，名字可以随便填；但登录名要和原来一样。
安装需要一段时间，如果屏幕变黑，那可能是因为键盘和鼠标长时间没动作而启动的屏幕保护，动动鼠标就恢复了，不要紧张，更不要强行关机。

安装完成后，按提示重启电脑。/home里的文件将完好无损。