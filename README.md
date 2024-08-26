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
echo "Hello." > A.txt
```

Confirm
```git
cd test
cat A.txt
```

#### 2. Git start & Add files to the staging area
```git
git init # git start
git add <file_name> or <.> # The . adds all files in the directory to the staging area.
```

#### 3. Files Commit
```git
git commit -m "<Any Message>"
```

![image](https://github.com/user-attachments/assets/de950500-b4d9-4bcd-a8df-73bec1fbcea4)


Confirm
```git
git status
```

![image](https://github.com/user-attachments/assets/5c06f30a-2734-481f-84e1-eb91a0539b21)

#### 4. Connect to a Remote Repo ↔ Git Repo(HTTPS Copy) e.g. "https://github.com/<git_name>/<repo_name>.git"
```git
git remote add origin https://github.com/shinho123/test01.git
```

Confirm
```git
git remote -v
```
![image](https://github.com/user-attachments/assets/6152d24a-6def-4066-8a97-ef6017b712d3)


#### 5. Data Push
```git
git push -u origin master
```

Error

![image](https://github.com/user-attachments/assets/483558e9-9034-4ed1-b2a8-6dbc9bc7a96c)

* This error message occurs due to a synchronization issue between the local branch and the remote branch. Specifically, the push is rejected because there are changes in the remote repository that are not present in the local repository.

Solve
```git
git pull origin master --rebase # Solve 1. rebase
git pull origin master --no-rebase # Solve 2. merge
```

Confirm
```git
git push -u origin master
```
![image](https://github.com/user-attachments/assets/009fbc40-1d08-44c1-80ad-63cbdfa0ff4b)


