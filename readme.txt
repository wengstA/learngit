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
1.git checkout --readme.txt
   ·没有提交到暂存区，回到版本库原样
   ·回退到暂存区后，修改前的状态
   
   test 2
  
