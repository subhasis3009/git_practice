shaws@LAPTOP-PNFHQ7HH MINGW64 ~
$ git --version
git version 2.28.0.windows.1

shaws@LAPTOP-PNFHQ7HH MINGW64 ~
$ pwd
/c/Users/shaws

shaws@LAPTOP-PNFHQ7HH MINGW64 ~
$ git config --global user.name "subhasis3009"

shaws@LAPTOP-PNFHQ7HH MINGW64 ~
$ git config --global user.email "subhasis3009@gmail.com"

shaws@LAPTOP-PNFHQ7HH MINGW64 ~
$ cd Documents

$ mkdir git_practice

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents
$ cd git_practice

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice
$ git init
Initialized empty Git repository in C:/Users/shaws/Documents/git_practice/.git/

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ ls
README.txt

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git add README.txt

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt


shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git commit -m "Add README.txt"
[master (root-commit) 66a4df4] Add README.txt
 1 file changed, 1 insertion(+)
 create mode 100644 README.txt

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git log
commit 66a4df49ca58f217ba0be1d02d41d9635ab8d59a (HEAD -> master)
Author: subhasis3009 <subhasis3009@gmail.com>
Date:   Fri Aug 21 09:19:55 2020 +0530

    Add README.txt

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git remote add origin https://github.com/subhasis3009/git_practice.git

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 238 bytes | 238.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/subhasis3009/git_practice.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.txt

no changes added to commit (use "git add" and/or "git commit -a")

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git add README.txt

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.txt


shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git commit -m "Update README.txt"
[master 43ab10c] Update README.txt
 1 file changed, 2 insertions(+), 1 deletion(-)

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$ git push -u origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 291 bytes | 291.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/subhasis3009/git_practice.git
   66a4df4..43ab10c  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

shaws@LAPTOP-PNFHQ7HH MINGW64 ~/Documents/git_practice (master)
$
