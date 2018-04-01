1. *Merge commits from another repo*
    
      ```bash
      git remote add remote1 <remote-url>
      git fetch remote1
      git checkout <working-branch>
      git merge remote1
      git remote rm remote1
      ```
    
  2. *Rename folder*
  
      ```bash
      git mv <old-name> tmp
      git mv tmp <new-name>
      ```
      
  3. *Delete last commit*
  
      ```bash
      git reset --hard HEAD~1
      ```
      
  4. *Get old version of 1 file*

      ```bash
      git checkout <commit hash> <path>
      ```
      
  5. *Change message of pushed commit*
  
   		```bash
       git rebase -i HEAD~<number of backward commit>
       # Select r at commit want to change message -> save -> edit message -> save -> push force
    	```
    
5. *Revert commit*

    ```bash
    git revert <commit-hash>
    # Create new commit with the inverse of the commit
    ```
