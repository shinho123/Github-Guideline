## Github Guideline

### Github Basic Terms

* Repository(레퍼지토리, 저장소) : 프로젝트의 파일과 변경 이력을 저장하는 장소이다. / 로컬 저장 장소와 원격 저장소로 나눌 수 있다.
* Branch(브랜치) : 독립적인 작업을 위한 분기이다. 브랜치를 사용하여 서로 다른 기능이나 버그 수정을 동시에 작업할 수 있다. 
* Commit(커밋) : 변경 사항을 기록하는 스냅샷이다. / 각 커밋은 고유한 해시 값으로 식별된다.
* Push(푸시) : 로컬 저장소의 변경 사항을 원격 저장소에 업로드한다.
* Pull(풀) : 원격 저장소의 변경 사항을 로컬 저장소로 가져와 병합한다.
* Fetch(페치) : 원격 저장소의 변경 사항을 로컬 저장소로 가져오지만, 병합하지는 않는다.
* Merge(병합) : 두 브랜치의 변경 사항을 하나로 통합한다. / 병합 커밋이 생성된다.
* Rebase(리베이스) : 브랜치의 커밋을 다른 브랜치의 최신 커밋 위로 재배치한다. / 커밋 히스토리를 선형으로 유지한다.
* Tag(태그) : 특정 커밋에 레이블을 붙인다. / 주로 릴리즈 버전을 표시하는 데 사용된다.
* Remote Repository(원격 저장소) : 네트워크를 통해 접근할 수 있는 저장소이다. / GitHib와 같은 서비스에 호스팅된다.
* Local Repository(로컬 저장소) : 사용자의 컴퓨터에 저장된 저장소이다.
* Fork(포크) : 다른 사용자의 원격 저장소를 복제하여 자신의 원격 저장소로 만든다. / 주로 오픈 소스 프로젝트에 기여할 때 사용한다.
* Pull Request(풀-리퀘스트) : 변경 사항을 원래 저장소에 병합해달라고 요청하는 기능이다. / 코드 리뷰와 협업에 사용된다.
* Issue(이슈) : 버그, 기능 요청, 작업 항목 등을 추적하는 데 사용되는 타겟이다.
* Wiki(위키) : 프로젝트와 관련된 문서를 작성하고 관리할 수 있는 공간이다.
* Actions(액션) : GitHub에서 제공하는 CI/CD 도구이다. / 자동화된 빌드, 테스트, 배포 작업을 수행할 수 있다.
* Release(릴리즈) : 소프트웨어의 특정 버전을 배포하는 기능이다. / 릴리즈 노트와 함께 배포 파일을 포함할 수 있다. 
* Contributor(기여자) : 프로젝트에 기여한 사람이다. 코드, 문서, 이슈 등을 통해 기여할 수 있다.
* Collaborator(협업자) : 저장소에 직접 접근하여 변경 사항을 추가할 수 있는 권한을 가진 사람이다.
* Commit Message(커밋 메시지) : 커밋에 대한 설명을 제공하는 메시지이디ㅏ. / 변경 사항의 목적과 내용을 설명한다. 
* Changes(변경 사항) : 파일의 추가, 수정, 삭제와 같은 변경 내용이다.
* Staging(스테이징) : 커밋할 파일을 선택하는 과정이다. 'git add' 명령어를 사용하여 파일을 스테이징 영역에 추가한다.
* Staging Area(스테이징 영역) : 커밋할 파일이 임시로 저장되는 영역이다. 인덱스라고도 불린다.
* Working Directory(작업 디렉토리) : 현재 작업 중인 파일이 있는 디렉토리이다. 로컬 저장소의 파일이 위치한다.
* HEAD : 현재 체크아웃된 브랜치나 커밋을 가리키는 포인터이다.
* Master Branch(마스터 브랜치) : 기본 브랜치로, 주로 배포 가능한 안정된 코드를 포함한다. / 많은 프로젝트에서 'main' 브랜치로 대체되고 있다. 
* Main Branch(메인 브랜치) : 기본 브랜치로, 주로 배포 가능한 안정된 코드를 포함한다. / 'master' 브랜치가 기본 브랜치로 설정된다.
* Default Branch(기본 브랜치) : 저장소에서 기본으로 사용되는 브랜치이다. 주로 'main' 또는 'master' 브랜치가 기본 브랜치로 설정된다.
* README File(리드미 파일) : 프로젝트에 대한 설명, 설치 방법, 사용 방법 등을 포함하는 파일이다. / 주로 'README.md' 형식으로 작성된다.
* .gitignore File(.gitignore 파일) : Git이 추적하지 않을 파일이나 디렉토리를 지정하는 파일이다. / 주로 빌드 아티팩트나 개인 설정 파일을 제외하는 데 사용된다.

### Github Basic Commander

* git init : 새로운 Git 저장소를 초기화한다. / 현재 디렉토리를 Git 저장소로 만든다.
* git clone : 원격 저장소를 로컬로 복제한다. / 원격 저장소의 모든 파일과 히스토리를 가져온다.
* git add : 변경 파일을 Staging Area에 추가한다. / 커밋할 파일을 선택한다.
* git commit : Staging된 변경 사항을 커밋한다. / 커밋 메시지를 포함하여 변경 사항을 기록한다.
* git push : 로컬 브랜치의 커밋을 원격 저장소에 푸시한다.
* git pull : 원격 저장소의 변경 사항을 가져와 로컬 브랜치에 병합한다.
* git fetch : 원격 저장소의 변경 사항을 가져오지만, 로컬 브랜치에 병합하지는 않는다.
* git merge : 두 브랜치를 병합한다. 병합 커밋을 생성하여 두 브랜치의 변경 사항을 통합한다.
* git rebase : 브랜치의 커밋을 다른 브랜치의 최신 커밋 위로 재배치 한다. / 커밋 히스토리를 선형으로 유지한다. 
* git status : 현재 작업 디렉토리의 상태를 보여준다. / 추적된 파일, 추적되지 않은 파일, Staging된 파일 등을 확인할 수 있다.
* git log : 커밋 히스토리를 보여준다. 각 커밋의 해시, 작성자, 작성 시간, 커밋 메시지 등을 확인할 수 있다.
* git branch : 브랜치를 생성, 삭제, 나열한다. / 현재 브랜치를 확인할 수 있다.
* git checkout : 브랜치를 전환하거나, 특정 커밋으로 작업 디렉토리를 업데이트한다.
* git tag : 특정 커밋에 태그를 추가한다. 태그는 주로 릴리즈 버전을 표시하는 데 사용된다.
* git remote : 원격 저장소를 관리한다. / 원격 저장소를 추가, 삭제, 나열할 수 있다.
* git diff : 변경 사항을 비교한다. 작업 디렉토리와 Staging Area, 또는 두 커밋 간의 차이를 보여준다.
* git stash : 현재 작업 중인 변경 사항을 임시로 저장하고, 작업 디렉토리를 깨끗하게 만든다. 나중에 다시 적용할 수 있다.
* git reset : 커밋 히스토리를 재설정한다. 특정 커밋으로 되돌리거나, Staging Area을 초기화 할 수 있다.
* git rm : 파일을 삭제하고, 삭제된 파일을 Staging Area에 추가한다. 
* git mv : 파일을 이동하거나 이름을 변경하고, 변경 사항을 Staging Area에 추가한다.

### The step-by-step instructions for synchronizing data between Git and a local repository


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


