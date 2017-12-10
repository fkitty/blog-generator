---
title: git操作
date: 2017-12-09 20:04:09
tags:
---
学git就是为了github

配置GitHub
这些key就是钥匙$ ll ~/.ssh

把锁安到账号上面 自己手里拿那把钥匙
上传上来的东西就是和钥匙配对的锁   你的机器上有个钥匙
每次git连接过来的时候这个钥匙就会自动插到这个锁里
如果是配对的就可以进去
一个钥匙打开后 可以看到很多仓库


输入第二个命令后按三次回车
用 ll ~/.ssh查看生成的文件
total 8
-rw-r--r-- 1 summer_taq 197121 3243 12月  7 13:38 id_rsa
-rw-r--r-- 1 summer_taq 197121  744 12月  7 13:38 id_rsa.pub



用cat ~/.ssh/id_rsa.pub查看内容，这个就是与钥匙配套的锁，
没有pub的就是钥匙

然后new key中
输入名字  这个锁的内容  然后输入github的内容，这个锁就添加好了


测试这个锁是否添加成功：cat ~/.ssh/know_hosts
但是win不支持cat命令




git log
git status -sb
创建 git init
加文件git add
提交git commit(一个commit的数是有32位的十六进制的数组成的字符串)



git log产看每次commit的信息
commit就是把每次add的信息给提交一下
add暂存区


origin:给ssh这个地址的字符串取一个名字叫origin

推送的时候那个仓库的文件不能是打开状态，不然就推不成功

下载仓库
拿到地址 git clone  进入对应的目录

你的远程被人更改了 要先pull 再push
git add 文件路径
git commit -m "信息"
git pull （相信我，你一定会忘记这一个命令）
git push




vim  如何退出vim:   esc  :  q  !



hexo new myfirsthexo
INFO  Created: ~/Desktop/myBlog/source/_posts/myfirsthexo.md

8.start 那个.md文件的路径
这样写start  ~/Desktop/myBlog/source/_posts/myfirsthexo.md
就可以编辑这个md文件了，注意命令生成的路径中的斜杠换个方向




tuoanqi.github.io是放上传博客后生成的代码的，一般不用动
blog-generator-是存放博客的地方

每次上传完博客后记得 add commit pull push
即：git add .
    git commit -m "第几次提交"
    git pull 
    git push



/Desktop/myBlog/source/_posts/Hexo的使用.md
/Desktop/myBlog/source/_posts/第三篇博客.md

