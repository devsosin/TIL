### Git Basic Command

Git 기본 명령어



### ㅇ 로컬 저장소

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



### ㅇ GitHub

#### git remote add origin : 주소 설정 

- git remote add origin 주소
  - repository (.git 추가)

``` shell
$ git remote add origin 주소.git
```



#### origin 초기화

- git remote remove origin

``` shell
$ git remote remove origin
```



#### git remote -v

- git remote
  - -v : origin 확인

``` shell
$ git remote -v
```



#### git push origin master

- git push origin master

``` shell
$ git push origin master
```



#### git reset

- git reset HEAD . : add 취소
- git reset --option HEAD^ : commit 취소
  - --soft : add 상태로 전환
  - --mixed : 기본 상태로 전환 (WD에 보존)
  - --hard : WD에서 삭제
  - HEAD~number : number 만큼 취소

```shell
$ git reset HEAD
$ git reset --soft HEAD^
```

