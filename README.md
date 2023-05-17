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
$ ^C

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch dev

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch
  dev
* main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch dev
Switched to branch 'dev'

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$ git branch
* dev
  main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$ git branch test

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$ git branch
* dev
  main
  test

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$ git branch --delete test
Deleted branch test (was 2f9d666).

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$ git branch
* dev
  main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (dev)
$
  
  ## bundle 2 exercise 1
  
  
HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch ft/bundle-2

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch
  dev
  ft/bundle-2
* main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch ft/bundle-2
Switched to branch 'ft/bundle-2'

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git commit -m "first commit by adding a paragraph"
[ft/bundle-2 2283721] first commit by adding a paragraph
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git add services.html

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git commit -m "second commit on new branch"
[ft/bundle-2 79028d1] second commit on new branch
 1 file changed, 2 insertions(+), 1 deletion(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 842 bytes | 93.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/shema-felix/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/bundle-2)
$
  ####
