Git learning:  
- [Git版本控制软件结合GitHub从入门到精通常用命令学习手册](http://www.oschina.net/question/1397765_166368)  
- [廖雪峰Git教程](http://www.liaoxuefeng.com/)


###migrate git repository from one to another
1). 从原地址克隆一份裸版本库，比如原本托管于 GitHub  
	git clone --bare git@git.oschina.net:cuilc/DroolDemo.git

2). 然后到新的 Git 服务器上创建一个新项目，比如 drools-demon  

3). 以镜像推送的方式上传代码到 drools-demon 服务器上。  
	git push --mirror git@github.com:cuilc/drools-demon.git

or   
	git commit -m "Change repo." # 先把所有为保存的修改打包为一个commit
	git remote remove origin # 删掉原来git源
	git remote add origin [YOUR NEW .GIT URL] # 将新源地址写入本地版本库配置文件
	git push -u origin master # 提交所有代码

###create a new repository on the command line
	echo "# drools-demon" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin git@github.com:cuilc/drools-demon.git
	git push -u origin master

