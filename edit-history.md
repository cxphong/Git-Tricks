1. *Merge commits from another repo*
    
      ```python
      git remote add remote1 <remote-url>
      git fetch remote1
      git checkout <working-branch>
      git merge remote1
      git remote rm remote1
      ```
    
  2. *Rename folder*
  
      ```python
      git mv <old-name> tmp
      git mv tmp <new-name>
      ```
      
  3. *Delete last commit*
  
      ```bash
      git reset --hard HEAD~1
      ```
