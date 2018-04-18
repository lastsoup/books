
# github使用
1、初始化   
下载git工具   
初始化配置   
$ git config --global user.name "lastsoup"   
$ git config --global user.email "qingtang166@qq.com"   
新建文件夹存放仓库   
初始化一个git库：$ git init   
克隆仓库：$ git clone https://github.com/lastsoup/books.git   
克隆分支仓库：$ git clone -b newbranch https://github.com/lastsoup/books.git   
2、分支操作   
查看分支：$ git branch   
新建分支：$ git branch newbranch   
切换到新分支：$ git checkout newbranch   
新分支发布在github：$ git push origin newbranch   
删除本地分支：$ git branch -d newbranch   
删除github分支：$ git push origin :newbranch    
3、发布   
切换到需要提交的分支下   
先提交文件：$ git add .   
查看状态：$ git status   
确定提交：$ git commit -a -m '新增txt文件'   
发布到github：$ git push/有分支：$ git push origin master   
4、回退   
回退命令：   
$ git reset --hard newbranch^         回退到上个版本   
$ git reset --hard newbranch~3        回退到前3次提交之前，以此类推，回退到n次提交之前   
$ git reset --hard commit_id     退到/进到 指定commit的sha码   
强推到远程：$ git push origin newbranch --force      
5、问题   
提示：Another git process semms to be running in this repository   
解决方案：进入项目文件夹下的 .git文件中（显示隐藏文件夹或rm .git/index.lock）删除index.lock文件即可   
提示：fatal: unable to access 'https://github.com/lastsoup/books.git/': Empty reply from server   
解决方案：重置本机git设置：$ git config --global credential.helper store   
# 电子书使用   
发布到分支gh-pages 访问https://lastsoup.github.io/books/
# 在线markdown编辑器
https://dillinger.io/
