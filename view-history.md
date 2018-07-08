###### View history
	- Full information
		git log

	- Minimize information
		git log --oneline --graph --decorate --all

	- Not full but enough information
		git log  --graph --pretty=format:"%h%x09%an%x09%ad%x09%s"

	- One branch
		git log --graph --oneline --decorate <branch name>

	- Only one file
		git log --follow <file path>
		git log --follow --oneline <file path>

	- What changed in one commit
		git show <commit hash>

	- List files changed in one commit
		git show --name-only <commit hash>

	- What changed of one file in one commit
		git show <commit hash> <file-path>

	- All tag
		git tag
		git log --tags --simplify-by-decoration --pretty="format:%ci %d"

	- Find commit file added
		git log --diff-filter=A -- <file-name>
	
	- View number line of codes of an author
		git log --author="Cao Xuan Phong" --pretty=tformat: --numstat | awk '{ add += $1; subs += $2; loc += $1 - $2 } END { printf "added lines: %s, removed lines: %s, total lines: %s\n", add, subs, loc }' 


###### Make alias to type less
		Edit file ~/.gitconfig
		
		-----------------------------------------------------------	
			[alias]
				tree = log --oneline --decorate --all --graph
		-----------------------------------------------------------

		Than just type 'git tree'
