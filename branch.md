### Create 1 branch	

```
	git branch <branch-name>
```

	- Move HEAD to new branch
		git checkout <branch-name>

	- Merge branch into
		git merge <name of branch want to merge into current branch>

	- Change branch name
		git branch -m old_branch new_branch         # Rename branch locally  

		# Dot 2 commands below if branch uploaded to remote  
		git push origin :old_branch                 # Delete the old branch    
		git push --set-upstream origin new_branch   # Push the new branch, set local branch to track the new remote

	- Delete branch
    	# Branch uploaded to remote
    	git branch -d <branch>
     	git push origin --delete <branch>

     	# Branch not uploaded to remote yet
     	git branch -D <branch>

	- Checkout remote branch
		git fetch
		git checkout <branch>

	- List all branch 
		git branch -a