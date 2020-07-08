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



#### git pull : GitHub에서 최근 Commit 불러오기

- git pull origin master

``` shell
$ git pull origin master
```



#### git clone : GitHub에서 프로젝트 복제 

- git clone origin

``` shell
$ git clone origin
```

