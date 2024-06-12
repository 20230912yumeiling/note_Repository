markdown 文本修饰语言，用特殊符号修饰正文效果<br>

## 修饰标识符\#

#标题修饰符（一级标题）
##（二级标题）
###（三级标题）
####（四级标题）
#####（五级标题）

##正文内容
  输入正文内容。但是你如果需要换行，用\<br\>标签

##修饰正文
  *一段测试文本*
  **一段测试文本**
  ***一段测试文本***
  ~~一段测试文本~~
  这是一段测试文本，将`关键字`，重点显示
#分割线
用\-\-\-表示分割线

---

##引用效果\> 表示
> 一级你自己就是一座金矿，关键在于如何挖掘和利用

>> 二级 苏格拉底

>>> 三级引用

>>>>四级引用

##列表修饰符
###无序列表 \*
*
###有序列表 1.
1. 网络工程
  1. 计算机网络
  2. 数据库
  3. 网络协议
2. 计算机科学与技术
  1. 计算机网络英文版
  2. 数据结构英文
##混合列表
1. 测试一级
   * 测试二级
   2. 测试三级
##


###表格
名称|技能|排行
--|:--:|--:
美羊羊|美|3
喜羊羊|聪明|1
沸羊羊|舔狗|2


##代码
```c
   #include<stdio.h>
   int main()
   {
   printf("nihao\n");
   return 0;
   }
```
```cpp
   #include<iostream>
```
```python
   import<os>
```
```bash
  echo "ceshi" 
  pwd
  ps aux 
  ls -l
```
#超链接技术 
##
[Github](https://www.github.com "点击访问 ")
##

#插入图片
##
![屏幕截图](C://Users//86137//Desktop//屏幕截图 2024-06-12 141206.png "悬停标题")
##
#查看方式 
1. 自带的typora
2. 浏览器插件
3.  github 查看，需要图片转公用链接地址 图床生成url
#Github<br>
##
1. 关键字查询 awesome,去此标签类别中查询项目<br>
2. python tutorial 查询资料，书籍 ，文档<br>
3. socket sample 查询对应技术的代码样本<br>
##
#Github三要素<br>
##
* Reppository
  1. 仓库是github项目存储基本单位
  2. 一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public,private
* Commit提交<br>
  程序员在整个开发周期，有大量的对代码的迭代，修改，都可以commit方式记录，便于程序员回溯代码，即使这些代码被删除，提交便于使用者
  
  观察整个工程的开发流程以及设计流程
* Branch分支<br>
  在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为master/main

  不仅可以管理代码存储，便于多人协作开发<br>

  [zhishi](https://postimage.me/image/1.d5EWf "悬停标题")

##
#仓库内容<br>
* **code** ,资源存储，代码资源，二进制，项目管理脚本，许可证等
* **issues** ,使用时遇到的bug或者进行提交 ，等待反馈

* **README** ,使用markdown 语言编写， 工程自述文件，开发进度，版本更新，使用介绍等等
* **LISENCE许可证**   GPL2.0 3.0 Apahce 2.0,Mit   这些许可证，给使用者最大使用权限以及最少的限制
#Git 软件，分布式控制系统
##
仓库管理软件，使用git 管理私人代码或企业代码
 ![zhishi2](https://postimage.me/image/Snipaste-2024-06-12-14-37-58.d5Jp3 "标题")

##


#设备认证
##
1. 如何让网站的账户与设备绑定，后续完成代码的管理，上传下载
```bash
 git init //创建本地仓库
 git config --list //查看git 配置文件
 git config --global user.email"邮箱"
 git config --global user.name "用户名"
 ssh—keygen -t rsa -C "注册邮箱" //创建本地图文
 //ssh 远程访问
 //去对应目录查找密文文件
 rsa.pub //复制密文，粘贴 settings->SSH key and GPG ->new ssh key ->粘贴
 ssh -T git@github.com //测试关联是否成功
```

2. 为目标仓库起别名，定位目标仓库，后续上传<br>
```bash
  git remote add origin "ssh地址 ”  //为ssh 仓库地址 创建别名为origin
  git remote remove origin  //删除origin 别名
```
##

#代码更新的依赖关系被破坏、
##
本地内容比云端新，完成更新 替换但是如果直接修改云端内容，导致，本地内容无法再次提交 <br>
先拉取git pull 云端内容，与本地内容合并或操作，而后再次推即可
```bash
   git pull --rebase origin master
   git rebase --skip //忽略本地内容，保存云端内容
   git rebase --abort //忽略本地内容，保存云端内容 
   git rebase --contiue //忽略本地内容，保存云端内容
```
#下载开源代码
##
```bash
  git clone "http 仓库地址" //下载开源项目code资源
```
#分支branch
##
关于分支的命令，创建分支，选择分支，合并分支 
