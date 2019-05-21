# git

> Git은 소스코드 항상(버전)관리 도구이다.

## 기본명령어

1 . 저장소(`repository`) 만들기

```bash
$ git init
Initialized empty Git repository in C:/Users/user/Desktop/TIL/.git/

user@pc16 MINGW64 ~/Desktop/TIL (master)
$
```

내가 원하는 폴더를 git으로 관리하는 저장소로 초기화한다. (`master`) 라는 표기를 통해 해당 폴더가  git repository라는 것을 확인할 수 있다.(더 정확하게는 해당 폴더에 숨긴 폴더로 .git이 있다.)



2. `git add` - 커밋할 목록에 추가하기

   ```bash
   $ git add .
   
   user@pc16 MINGW64 ~/Desktop/TIL (master)
   $ git status
   On branch master
   
   No commits yet
   
   Changes to be committed:
     (use "git rm --cached <file>..." to unstage)
   
           new file:   git.md
   
   ```

   `git add.`에서  `.`은 현재 디렉토리를 뜻하는 리눅스 표기법이다. 현재 디렉토리의 변경 사항들을 모두 커밋할 목록에 담아둔다는 뜻이다.

   `git add git.md`라고 하면, 특정 파일만 올릴 수도 있고, `git add myfolder/`라고 하면 , 특정 폴더를 모두 담아둘 수도 있다.

3. 커밋

   ```bash
   $ git commit -m '커밋메세지'
   ```

   커밋은 버전의 이력을 남기는 것이다. 커밋할 목록에 있는 내용들을 버전에 포함시킨다.(untracked / 목록에 없는 것은 포함 안됨.)

4.  커밋 이력 확인하기

   ```bash
   $ git config --global user.email '32142190@dankook.ac.kr'
   
   user@pc16 MINGW64 ~/Desktop/TIL (master)
   $ git config --global user.name 'godee95'
   
   user@pc16 MINGW64 ~/Desktop/TIL (master)
   $ git commit -m 'Git 기초 명령어 정리'
   [master (root-commit) b005623] Git 기초 명령어 정리
    1 file changed, 32 insertions(+)
    create mode 100644 git.md
   
   $ git log
   commit b0056231ca884f635bc481c9f2830bc653970c31 (HEAD -> master)
   Author: godee95 <32142190@dankook.ac.kr>
   Date:   Tue May 21 12:39:49 2019 +0900
   
       Git 기초 명령어 정리
   
   ```

   

5. **git상태** **확인하기**

   ```bash
   $ git status
   ```

   CLI(Command Line Interface)에서는 현재 상태를 확인하기 위해서 지속적으로 확인해야 한다.

6. 

7. 



