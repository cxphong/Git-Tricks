###### Stash & Clean
	- Ignore all modified (Becareful it can't undo)
		git checkout .

	- Ignore 1 modified file
		git checkout <file-name>

<<<<<<< HEAD:stage.md
	- Ignore a part of modified file

	- Add all mofified into stage
=======
	- Add mofified into stage
>>>>>>> 0d1f141f0bb5205b37a82e91aec0fa6e021bd233:stash-clean.md
		git add -A

	- Get back deleted file
		git checkout <file-name>

	- Unstage all
		git reset HEAD .

	- Unstage 1 file
		git reset HEAD <file-name>
