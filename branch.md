#### Create 1 branch	

```php
	git branch <branch-name>
```

#### Move HEAD to new branch

```php
	git checkout <branch-name>
```

#### Merge branch into

```php
	git merge <name of branch want to merge into current branch>
```

#### Change branch name

```php
		git branch -m old_branch new_branch         # Rename branch locally  

		# Dot 2 commands below if branch uploaded to remote  
		git push origin :old_branch                 # Delete the old branch    
		git push --set-upstream origin new_branch   # Push the new branch, set local branch to track the new remote
```

#### Delete branch

``php
    	# Branch uploaded to remote
    	git branch -d <branch>
     	git push origin --delete <branch>

     	# Branch not uploaded to remote yet
     	git branch -D <branch>
```
#### Checkout remote branch

```php
		git fetch
		git checkout <branch>
```
		
#### Pull

```php
		git pull
		git pull origin master
		git pull origin master --allow-unrelated-histories
```

#### List all branch 

```php
		git branch -a
```
