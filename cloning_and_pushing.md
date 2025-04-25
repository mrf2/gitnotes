# Cloning a repository and pushing new codes
1. At first clone the required repository by `git clone https://github.com/mrf2/gitnotes.git`
2. Check if remote is set by using `git remote -v`
	- `remote` is a Git command to manage remotes (like GitHub URLs).
	- `-v` `(--verbose)` - shows full URLs for each remote (for both fetch and push directions).
	# If nothing is listed, add remote:
	```bash
	git remote add origin http://github.com/mrf2/reponame.git

	- `add` - Adds a new remote
	- `origin` - The standard alias name Git uses for the remote repository.
	- The USL is the HTTPS or SSH path to HitHub repo.
3. See which branch your're on
	```bash
	git branch

	- Shows all local branches
	- The current branch is market with an asterisk `*`.

	If another branch is need, create it and switch to the new branch:
	```bash
	git checkout -b new-branch

	- `checkout` - Switches to a branch
	- `b` - Creates a new branch and switch to it immediately
	- `new-branch` - The name of the branch beging created
4. Add all changes to the staging area
	```bash
	git add .
	
	- `add` - Tess Git to include changes in the next commit.
	- `.` - Means **all files in the current directory"

	We can also add a specifc file by it's name:
	```bash
	git add path/to/file.txt
5. Commit your changes
	```bash
	git commit -m "inbox directory added"
	
	- `commit` - Saves the staged changes as a new commit.
	- `-m` - Allows us to provide the commit message directly.
	- `"inbox directory added`" - A short summary of what changed.
6. Check what's going on
	```bash
	git status

	# This shows:
		- The current branch
		- If any files have been modified, staged, untracked
		- Whether branch is ahead/behind the remote
		- If upstream tracking is missing or broken
