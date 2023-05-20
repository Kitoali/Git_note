# 目的
代码的备份，回滚，协同开发，追溯

## .bashrc 配置快捷键
#输出git提交日志
alias git-log='git log --pretty=oneline --all --graph --abbrev-commit'
#查找当前文件夹所有文件快捷键
alias ll = 'ls -al'
![image](https://github.com/Kitoali/Git_note/assets/54657765/f936537f-7dd9-4d58-9a49-e92001248e1d)


### 文件的提交 
 ![image](https://github.com/Kitoali/Git_note/assets/54657765/062b1323-a89e-48d4-abf4-bcce96635f59)

###通配符提交的方式忽略部分类型，或某个的文件的方法，一般通过复制.gitignore文件到仓库即可无需手写
 
![image](https://github.com/Kitoali/Git_note/assets/54657765/272822a4-1543-47d8-b9f2-5d43b5ada4b7)
![image](https://github.com/Kitoali/Git_note/assets/54657765/5ebfafa1-b2f4-4864-873c-4798bbea1377)

 
### 版本回滚方式
![image](https://github.com/Kitoali/Git_note/assets/54657765/16b7790f-f50b-47e5-a432-5e19a0f988b6)
当清空命令后
![image](https://github.com/Kitoali/Git_note/assets/54657765/f236d027-24a7-427a-b504-0488c62a28dc)
git 提交后都有记录，只要别把log文件删了
![image](https://github.com/Kitoali/Git_note/assets/54657765/ffed063d-9b9e-4eaa-b202-8a3c0a8b3624)

小结：
	a. 要想回到过去，必须先得到commit id，然后通过git reset –hard 进行回退；
	b. 要想回到未来，需要使用git reflog进行历史操作查看，得到最新的commit id；
	c. 在写回退指令的时候commit id可以不用写全，git自动识别，但是也不能写太少，至少需要写前4位字符；





