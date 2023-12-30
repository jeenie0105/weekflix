  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git add index.html

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git commit -m "div 추가"
[master ce23807] div 추가
 1 file changed, 6 insertions(+), 1 deletion(-)

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git log
commit ce238075ab79886e6f220e7c8d49bfeaa1b128d1 (HEAD -> master)
Author: jeenie0105 <jeenie2805@gmail.com>
Date:   Sat Dec 30 13:47:47 2023 +0900

    div 추가

commit 92be699d4ef7ce91f1f990e8644a043ac6a09b17
Author: jeenie0105 <jeenie2805@gmail.com>
Date:   Sat Dec 30 13:43:28 2023 +0900

    git commit test

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ ls -a
./  ../  .git/  index.html

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git config
usage: git config [<options>]

Config file location
    --[no-]global         use global config file
    --[no-]system         use system config file
    --[no-]local          use repository config file
    --[no-]worktree       use per-worktree config file
    -f, --[no-]file <file>
                          use given config file
    --[no-]blob <blob-id> read config from given blob object

Action
    --[no-]get            get value: name [value-pattern]
    --[no-]get-all        get all values: key [value-pattern]
    --[no-]get-regexp     get values for regexp: name-regex [value-pattern]
    --[no-]get-urlmatch   get value specific for the URL: section[.var] URL
    --[no-]replace-all    replace all matching variables: name value [value-pattern]
    --[no-]add            add a new variable: name value
    --[no-]unset          remove a variable: name [value-pattern]
    --[no-]unset-all      remove all matches: name [value-pattern]
    --[no-]rename-section rename section: old-name new-name
    --[no-]remove-section remove a section: name
    -l, --[no-]list       list all
    --[no-]fixed-value    use string equality when comparing values to 'value-pattern'
    -e, --[no-]edit       open an editor

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git branch -M master

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git remote add origin https://github.com/jeenie0105/WeekDay03.git

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git push -u origin master
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 860 bytes | 860.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/jeenie0105/WeekDay03.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git log
commit ce238075ab79886e6f220e7c8d49bfeaa1b128d1 (HEAD -> master, origin/master)
Author: jeenie0105 <jeenie2805@gmail.com>
Date:   Sat Dec 30 13:47:47 2023 +0900

    div 추가

commit 92be699d4ef7ce91f1f990e8644a043ac6a09b17
Author: jeenie0105 <jeenie2805@gmail.com>
Date:   Sat Dec 30 13:43:28 2023 +0900

    git commit test

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git add .

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git commit -m "한글 수정하여 추가"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$ git push -u origin master
Everything up-to-date
branch 'master' set up to track 'origin/master'.

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3/Day03_1230 (master)
$
 *  History restored 


희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3
$ git add .
fatal: not a git repository (or any of the parent directories): .git

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3
$ git commit -m "한글 수정하여 추가"
fatal: not a git repository (or any of the parent directories): .git

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3
$ git push -u origin master
fatal: not a git repository (or any of the parent directories): .git

희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3
$
 *  History restored 


희진@DESKTOP-TEIOKGF MINGW64 ~/Desktop/개발일기/Frontend_3
$