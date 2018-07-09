# usage: 
	git [--version] [--help] [-C <path>] [-c name=value]
		[--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
		[-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
		[--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
		<command> [<args>]

These are common Git commands used in various situations:

### start a working area (see also: git help tutorial)
	clone      Clone a repository into a new directory
	init       Create an empty Git repository or reinitialize an existing one

### work on the current change (see also: git help everyday)
	add        Add file contents to the index
	mv         Move or rename a file, a directory, or a symlink
	reset      Reset current HEAD to the specified state
	rm         Remove files from the working tree and from the index

### examine the history and state (see also: git help revisions)
	bisect     Use binary search to find the commit that introduced a bug
	grep       Print lines matching a pattern
	log        Show commit logs
	show       Show various types of objects
	status     Show the working tree status

### grow, mark and tweak your common history
	branch     List, create, or delete branches
	checkout   Switch branches or restore working tree files
	commit     Record changes to the repository
	diff       Show changes between commits, commit and working tree, etc
	merge      Join two or more development histories together
	rebase     Reapply commits on top of another base tip
	tag        Create, list, delete or verify a tag object signed with GPG

### collaborate (see also: git help workflows)
	fetch      Download objects and refs from another repository
	pull       Fetch from and integrate with another repository or a local branch
	push       Update remote refs along with associated objects

### help

	'git help -a' and 'git help -g' list available subcommands and some
	concept guides. See 'git help <command>' or 'git help <concept>'
	to read about a specific subcommand or concept.



### Demo

	git add .
	git commit -m "message"
	git pull
	git push
	
	git checkout -b dev
	git push origin dev:dev
	
	git branch -vv
	git branch -d dev
	git push origin :dev
	
	git tag --list
	git tag v1.0.0
	git push origin v1.0.0:v1.0.0
	git tag -d v1.0.0
	git push origin :v1.0.0
	
	git checkout -- filename
	git pull origin dev
	
	## Git 全局设置:
	git config --global user.name "username"
	git config --global user.email "email@example.com"

	## 创建git仓库
	mkdir project
	cd project
	git init
	touch README.md
	git add README.md
	git commit -m "first commit"
	git remote add origin https://gitee.com/uniqid/project.git
	git push -u origin master
	
	### 已有项目
	cd existing_git_repo
	git remote add origin https://gitee.com/uniqid/project.git
	git push -u origin master

	## git迁移
	git clone --bare git://github.com/username/project.git
	cd project.git
	git push --mirror git@gitcafe.com/username/newproject.git
	
	

