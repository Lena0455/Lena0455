
lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep
$ git init
Initialized empty Git repository in C:/Users/lenchik/Desktop/myrep/.git/

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git add .

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   text.txt


lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git commit
hint: Waiting for your editor to close the file... unix2dos: converting file C:/Users/lenchik/Desktop/myrep/.git/COMMIT_EDITMSG to DOS format...
dos2unix: converting file C:/Users/lenchik/Desktop/myrep/.git/COMMIT_EDITMSG to Unix format...
Aborting commit due to empty commit message.

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git config --global user.email
zavyalovalena28@gmail.com

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ $ git config --global user.name
bash: $: command not found

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git config --global user.name
Lena Zavyalova

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   text.txt


lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git commit
hint: Waiting for your editor to close the file... unix2dos: converting file C:/Users/lenchik/Desktop/myrep/.git/COMMIT_EDITMSG to DOS format...
dos2unix: converting file C:/Users/lenchik/Desktop/myrep/.git/COMMIT_EDITMSG to Unix format...
[main (root-commit) 4a6c994] comment to our commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 text.txt

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git log
commit 4a6c994c356ba4b7f6428d5c4eaa3c2dbaa54ed8 (HEAD -> main)
Author: Lena Zavyalova <zavyalovalena28@gmail.com>
Date:   Mon Apr 4 10:55:15 2022 +0300

    comment to our commit

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   text.txt

no changes added to commit (use "git add" and/or "git commit -a")

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git add .

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   text.txt


lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git commit -m "commit 2"
[main 37c6898] commit 2
 1 file changed, 1 insertion(+)

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git add .

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git commit "Добавили .gitignore"
error: pathspec 'Добавили .gitignore' did not match any file(s) known to git

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore


lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git log
commit 37c68985b5f27fc0a95ed15b9cfecdf787bf7ad3 (HEAD -> main)
Author: Lena Zavyalova <zavyalovalena28@gmail.com>
Date:   Mon Apr 4 11:00:07 2022 +0300

    commit 2

commit 4a6c994c356ba4b7f6428d5c4eaa3c2dbaa54ed8
Author: Lena Zavyalova <zavyalovalena28@gmail.com>
Date:   Mon Apr 4 10:55:15 2022 +0300

    comment to our commit

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   text.txt


lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git add .

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git commit -m "first commit"
[main bb096eb] first commit
 2 files changed, 1 insertion(+), 1 deletion(-)
 create mode 100644 .gitignore

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git remote add origin https://github.com/Lena0455/Lena0455.git

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git push -u origin main
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/Lena0455/Lena0455.git/'

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git status
On branch main
nothing to commit, working tree clean

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$ git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (9/9), 691 bytes | 691.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Lena0455/Lena0455.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

lenchik@DESKTOP-MKVM4JQ MINGW64 ~/Desktop/myrep (main)
$
