###### View history
	- Full information
		git log

	- Minimize information
		git log --online --graph --decorate --all

	- Not full but enough information
		git log  --graph --pretty=format:"%h%x09%an%x09%ad%x09%s"

	- One branch
		git log --graph --online --decorate <branch name>

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


###### Make alias to type less
		Edit file ~/.gitconfig
		
		-----------------------------------------------------------	
			[alias]
				tree = log --oneline --decorate --all --graph
		-----------------------------------------------------------

		Than just type 'git tree'