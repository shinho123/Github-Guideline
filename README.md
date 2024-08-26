## Github Guideline

### Github Basic Terms

* Repository
* Branch
* Commit
* Push
* Pull
* Fetch
* Merge
* Rebase
* Tag
* Remote Repository
* Local Repository
* Fork
* Pull Request
* Issue
* Wiki
* Actions
* Release
* Contributor
* Collaborator
* Commit Message
* Changes
* Staging
* Staging Area
* Working Directory
* HEAD
* Master Branch
* Main Branch
* Default Branch
* README File
* .gitignore File

### Github Basic Commander

* git init
* git clone
* git add
* git commit
* git push
* git pull
* git fetch
* git merge
* git rebase
* git status
* git log
* git branch
* git checkout
* git tag
* git remote
* git reset
* git rm
* git mv

### the step-by-step instructions for synchronizing data between Git and a local repository


#### 1. Initialize a Local Repository → 'test'
```git
mkdir test
cd test
echo "Hello. Welcome" > A.txt
```

confirm
```git
cd test
cat A.txt
```

#### 2. Git start & Add files to the staging area
```git
git init # git start
git add <file_name> or <.> # The . adds all files in the directory to the staging area.
```

#### 3. files Commit
```git
git commit -m "<Any Message>"
```
confirm
```git
git status
```

Connect to a Remote Repo ↔ Git Repo(HTTPS Copy) e.g. "https://github.com/<git_name>/<repo_name>.git"
