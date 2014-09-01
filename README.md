##我是demo

一个完整的demo，请参照可重复使用的无线点火器

欲呈现的效果为：https://www.zybuluo.com/plantpark/note/24062

各位只需要将md代码提交到github

##github使用教程：
windows https://github.com/JiapengLi/GitTutorial 

mac/linux 等，自行google吧

##github unix cmd 使用教程

###pull request 使用教程

https://www.zybuluo.com/plantpark/note/24419


###第一次使用github，添加ssh认证

git init 

ssh-keygen -t rsa -C "your_email@example.com"

>Enter file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]

直接回车


此处输入passhprase与否均可

>Enter passphrase (empty for no passphrase): [Type a passphrase]
>Enter same passphrase again: [Type passphrase again]

回车后出现如下提示:

>Your identification has been saved in /Users/you/.ssh/id_rsa.
>Your public key has been saved in /Users/you/.ssh/id_rsa.pub.
>The key fingerprint is:
>01:0f:f4:3b:ca:85:d6:17:a1:7d:f0:68:9d:f0:a2:db your_email@example.com

如此，ssh key就保存到了“/Users/you/.ssh/id_rsa.pub.”文件内，

直接cat /Users/you/.ssh/id_rsa.pub ,将输出的结果复制到如图所示的地方保存即可。


![](https://github-images.s3.amazonaws.com/help/settings/ssh-key-paste.png)

(设置--->SSH Keys---->Add SSH key)




###就将仓库clone到本地

git clone git@github.com:huohuaioio/article.git

###本地仓库增加新文件后如此流程操作

git add *

git commit -m "first commit"

git push -u origin master

###当遇到多人同时更新github仓库时，需要先将github仓库更新到本地，然后在执行第二个步骤。
git fetch --all

git reset --hard origin/master

git pull origin master
