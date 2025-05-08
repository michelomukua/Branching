## Git Branching Practice

Git Cheat sheet and branching practice

### Basic Commands
* `git init` -initialize local git repo in current folder( working directory)
* `git add .` - stage all changes for commit
* `git commit -m "message"` - commit staged changes to local repo

### Info Commands
* ` git staus` - show current status of working directory
* `git log` - show local commit history
* `git log --oneline` show local commit history, compact format



### Branching Commands
* `git branch`- list local branches
* `git branch branchName` -create new branch 'branchName'
* `git checkout branchName`


### Remote Commands
* `git remote add alias URL` -connect local repo to remote, using nane 'alias' for remote repo 'URL'
* `git push alias branchName` -push local commits to remote repo 'alias' on branch 'branchName'


### Git Branch Workflow
1. Go to local 'main' branch
	
	git checkout main

2. Pull remote main

	git pull origin main

3. Create and check out new branch

	git checkout -b featureName

1. work on your branch, committing frequently
1. when task is complete, pull main into your branch and fix merge conflicts

git add .
git commit  -m "Complete feature"
git pull origin main

fix any merge conflicts and commit the fix.

1. Push to your branch

	git push origin featureName

1. Create pull request