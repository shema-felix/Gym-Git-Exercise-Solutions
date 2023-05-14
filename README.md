# Gym-Git-Exercise-Solutions

#bundle 1

#exercise 1

'''bash
HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git init
Initialized empty Git repository in C:/Users/HP/Desktop/gym/.git/

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        web.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (master)
$ git branch -m master main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git config --global init.default main
warning: init.default has multiple values
error: cannot overwrite multiple values with a single value
       Use a regexp, --add or --replace-all to change init.default.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        web.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   web.html


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   web.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   web.html


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git diff
diff --git a/web.html b/web.html
index 96e2bc7..c4df6e2 100644
--- a/web.html
+++ b/web.html
@@ -12,6 +12,7 @@
       <div class=" grid-item-1">a</div>
       <div class=" grid-item-2">b</div>
       <div class=" grid-item-3">c</div>
+      <div class=" grid-item-4">d</div>




HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git add web.html

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git commit -m "first commit -adding another grid item"
[main (root-commit) 2f9d666] first commit -adding another grid item
 1 file changed, 22 insertions(+)
 create mode 100644 web.html

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git commit -m "first commit -adding another grid item"
On branch main
nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git remote add origin https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch -M main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 490 bytes | 245.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$
