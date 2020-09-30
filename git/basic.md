### Git Basic Command

Git 기본 명령어



### ㅇ 로컬 저장소 My Computer

### git init

현재 WD를 git으로 관리하겠다 선언

※ 프로젝트 단위로 git init 하는 것이 좋다 (상위에서 다시 git init 하는 경우는 없어야함.)
repository 별로 하나씩 추가

``` shell
$ git init
```



#### git add 파일 or .(현재 폴더)

- git add : 깃 저장소에 등록
  - . 하위 디렉토리 전부

```shell
$ git add .
```



#### git commit

- git commit : 깃 로그에 커밋

``` shell
$ git commit
```



#### git log

- git log : git에 commit 내역 확인

```shell
$ git log
```



#### git status

- git status : 현재 git 상태

``` shell
$ git status
```



#### git reset

- git reset HEAD . : add 취소
- git reset --option HEAD^ : commit 취소
  - --soft : add 상태로 전환
  - --mixed : WD에 보존
  - --hard : WD에서 삭제
  - HEAD~number : number 만큼 commit 취소

```shell
$ git reset HEAD
$ git reset --soft HEAD^
```



### ㅇ 원격저장소 GitHub

#### git remote : GitHub에 연결 

- add origin 주소 : GitHub 주소 설정
  - repository (.git 추가)

``` shell
$ git remote add origin 주소.git
```



- remove origin : GitHub 주소 초기화

``` shell
$ git remote remove origin
```



- -v  origin 확인

``` shell
$ git remote -v
```



#### git push : GitHub에 등록

- git push origin master

``` shell
$ git push origin master
```



#### git pull : GitHub에서 처리되지 않은 Commit 불러오기

- git pull origin master

``` shell
$ git pull origin master
```





## GitHub Cooperation Method

#### 협엽프로젝트 진행 시 깃허브 기반 프로젝트 관리 방법


#### git clone : GitHub에서 프로젝트 복제 (1회만)

- git clone <origin>

``` shell
$ git clone origin
```



#### git branch: 협업 프로젝트용 branch 생성 (임시 add, commit용)

- git branch <name>

``` shell
$ git branch sosin
```



#### git checkout: 협업 프로젝트 branch로 전환 (임시 add, commit)

- git checkout <branch>
- git checkout -b <branch> 생성도 함께 진행

``` shell
$ git checkout sosin(master)
```



##### 개인 프로젝트 진행하듯이 동일하게 add, commit 작업

##### branch master로 전환



#### git fetch: 강제 버전 맞추기 1

- git fetch --all

``` shell
$ git fetch --all
```



#### git reset: 강제 버전 맞추기 2

- git reset --hard master

``` shell
$ git reset --hard master
```



#### git merge: 협업 프로젝트 commit 병합 

- git merge <commit code> (branch의 git status에서 git log 확인하여 복사)

``` shell
$ git merge 6d6a6932ce4cfd18d48cfd5c3fa3cbd4546202bf
```



##### push origin하면 원격저장소에 업로드
