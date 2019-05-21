# Git

> Git은 소스코드 형상(버젼)관리 도구이다.

## 기본명령어

> 1. 저장소(`repository`) 만들기
>
>    ```bash
>    $ git init
>    Initialized empty Git repository in C:/Users/user/Desktop/TIL/.git/
>    $ user@PC13 MINGW64 ~/Desktop/TIL (master)
>    ```
>
>    내가 원하는 폴더를 git로 관리하는 저장소로 초기화한다.(`master`)라는 표기를 통해 git repository라는 것을 확인할 수 있다.(해당폴더에 숨김폴더로 `.git`가 있다.)
>
> 2.  `git add` - 커밋할 목록에 추가하기
>
>    ``` bash
>    $ git add .
>    
>    $ user@PC13 MINGW64 ~/Desktop/TIL (master)
>    $ git status
>    On branch master
>    
>    No commits yet
>    
>    Changes to be committed:
>      (use "git rm --cached <file>..." to unstage)
>    
>            new file:   Git.md
>    
>    ```
>
>    `git add .`에서 `.`은 현재 디렉토리를 뜻하는 리눅스 표기법이다. 현재 디렉토리의 변경 사항들을 모두 커밋할 목록에 담아둔다는 뜻이다.
>
>    `git add git.md`라고 하면, 특정 파일만 담아둘 수도 있고, `git add myfolder/` 라고하면, 특정 폴더를 모두 담아둘 수도 있다.
>
> 3. 커밋
>
>    ``` bash
>    $ git commit -m '커밋메세지'
>    
>    $ git commit -m 'Git'
>    [master (root-commit) 4a23b61] Git
>     1 file changed, 17 insertions(+)
>     create mode 100644 Git.md
>    
>    ```
>
>    커밋은 버전의 이력을 남기는 것이다. 커밋할 목록에 잇는 내용들을 버전에 포함시킨다.(add한 파일들만)
>
> 4. 커밋 이력 확인하기
>
>    ``` bash
>    user@PC13 MINGW64 ~/Desktop/TIL (master)
>    $ git log
>    commit 4a23b61b353d6a547dba55deb2a1a7cd14218f7c (HEAD -> master)
>    Author: Minho <fastz123@naver.com>
>    Date:   Tue May 21 12:39:54 2019 +0900
>    
>        Git
>    
>    ```
>
> 5. **git 상태 확인하기**
>
>    ```bash
>    $ git status
>    ```
>
>    CLI에서는 현재상태를 확인하기 위해서 지속적으로 확인해야 한다.

