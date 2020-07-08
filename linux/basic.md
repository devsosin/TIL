### Linux 기초 문법

Linux 기본 문법 정리 

$ = Terminal

#### └ 현재 폴더 위치

- pwb (print working directory)

```shell
$ pwb
```

#### └ 폴더 변경

- cd (change directory)

```shell
$ cd <이동하고 싶은 위치>
```

#### └ 현재 WD 내 파일, 폴더 리스트

- ls (list)
  - -a 옵션은 숨긴파일까지 출력

```shell
$ ls -a
```

#### └ 파일 생성

- touch

``` shell
$ touch <파일이름>
```

#### └ 파일 삭제

- touch

``` shell
$ touch <파일이름>
```

#### 파일 삭제

- rm (remove)
  - -r 폴더 삭제

``` shell
$ rm <파일이름>
$ rm -r <폴더이름>
```

#### └ 텍스트 파일 편집

- vi 

``` shell
$ vi <파일이름>
```

##### 텍스트 파일 편집 중 명령어

- i (insert) : 편집
- esc : 편집 종료
- : : 명령어 상태로 변경
- wq : 저장 후 종료

#### └ 텍스트 파일 보기

- cat

``` shell
$ cat <파일이름>
```

