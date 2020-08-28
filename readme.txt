Git is a distributed version control system.
Git is a free software distributed under the GPL.
Git has a mutable index called stage.
Git has a mutable index called stage.
Git tracks changes of files.
工作区——add——暂存区——commit——仓库:
	1.git add "file.name"
	2.git commit -m"commit files in the stage"
版本回退：
1.check 版本号：
	git log--onrline
	git reflog
2.回退
	git reset --hard 1049a
	
git status 内容解读：
	Untracked files:这个文件还没有被提交过——git add
	
撤销修改：
1.add × commit×
   手动删除/
   git checkout --readme.txt
   ·没有提交到暂存区，回到版本库原样
   ·回退到暂存区后，修改前的状态
 2.add √ commit×
  git reset HEAD readme.txt
      清除暂存区
  git checkout -- readme.txt
      清除工作区
	  
删除文件

1.rm <file>/手动删除——工作区删除
2.git rm test.txt——版本库删除
3.git commit -m"remove test.txt'——提交删除
 ps:还原删除（已经提交过文件的情况）
 git cheout --  text.txt

git & github
1.添加远程仓库
  git remote add origin git@github.com:wengstA/learngit.git
	远程仓库的名字是origin
2.push 到远程仓库上
  git push -u origin master
	当前分支master和远程的master分支关联起来
3.从远程仓库克隆
  git clone git@github.com:wengstA/hello-world.git'
