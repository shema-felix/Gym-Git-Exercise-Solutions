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
  
  
  ### bundle 2 exercise 2
  
  
  $ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git pull
Already up to date.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git commit -m "commiting adress"
[main 1e6144d] commiting adress
 1 file changed, 1 insertion(+)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git switch main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git commit "third commmit"
error: pathspec 'third commmit' did not match any file(s) known to git

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git commit -m "third commit"
[ft/service-redesign 1a7ba88] third commit
 1 file changed, 8 insertions(+), 1 deletion(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 358 bytes | 39.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
   cc249df..1a7ba88  ft/service-redesign -> ft/service-redesign

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git diff

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git diff

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 303 bytes | 101.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
   3d80277..1e6144d  main -> main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git diff

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git merge
HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main|MERGING)
$ git merge
Already up to date.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ 

#######
  
  #bundle 3
  
  #exercise 1
  
  
HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch -c ft/team-page
Switched to a new branch 'ft/team-page'

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* ft/team-page
  main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git commit -m  "team page commit"
[ft/team-page 89068f2] team page commit
 1 file changed, 1 insertion(+), 2 deletions(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 316 bytes | 105.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/shema-felix/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch ft/contact-page

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* main

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git switch ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git log
commit 89068f285415c88050ee28da712da3a7d0dc4c90 (HEAD -> ft/team-page, origin/ft/team-page)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 19:02:42 2023 +0200

    team page commit

commit 5319a1f8e81d982974620703b356e5e01a71df18 (origin/main, main, ft/contact-page)
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Thu May 18 18:52:37 2023 +0200

    Update README.md

commit bdcb76beff61e836043eb575bcd661ff4d3bd451
Merge: 1e6144d 1a7ba88
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:49:43 2023 +0200

    Merge branch 'ft/service-redesign'

commit 1a7ba888c45dbfab7db947c22d71ef358610c802 (origin/ft/service-redesign, ft/service-redesign)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:39:43 2023 +0200

    third commit

commit 1e6144dea5f86b106c0f892ed6622cf265e4869a
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:35:29 2023 +0200

    commiting adress

commit 3d802774b017c267e2a8789d8fd88df7bce9d970
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:31:07 2023 +0200

    2nd list

commit 0a81061db6f1558af7af801f3f402483635507e1
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:20:13 2023 +0200

    unordered list

commit cc249df1760c04c5d41c8c5a4ca12ec431b8a507
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Wed May 17 19:09:18 2023 +0200

    Update README.md

commit b35f9075b375e6968e0f87bb6cd7a30fb1a7c8f6
Merge: 58a8cd3 79028d1
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Wed May 17 19:03:44 2023 +0200

    Merge pull request #1 from shema-felix/ft/bundle-2

    new feature

commit 79028d14261655bb4d7acaa0a4fa8477c4e6433c (origin/ft/bundle-2, ft/bundle-2)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 18:33:07 2023 +0200

    second commit on new branch

commit 2283721efcc08f1fed48abac0ee52e93266117ae
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 18:09:53 2023 +0200

    first commit by adding a paragraph

commit 58a8cd3e4a033881a401a48e32478a97ca91ddbe
Author: shema-felix <shemabfelix@gmail.com>
Date:   Mon May 15 22:31:26 2023 +0200

    commiting changes to my file

commit 694da368a78f4834bf1ac2ef81b1dd9c9972b91e (origin/dev)
Merge: 98883ae 3852944
Author: shema-felix <shemabfelix@gmail.com>
Date:   Mon May 15 22:22:24 2023 +0200

    Merge branch 'main' of https://github.com/shema-felix/Gym-Git-Exercise-Solutions

commit 98883aefaa0dfa71f8e1f26eca0463d148b43565
Author: shema-felix <shemabfelix@gmail.com>
Date:   Mon May 15 22:04:10 2023 +0200

    commiting changes in home page

commit 3abdc7affb1060851423cbc250373e1c123ebe66
Author: shema-felix <shemabfelix@gmail.com>
Date:   Mon May 15 21:39:10 2023 +0200

    fourth commit

commit 078b060cbbeff5cdf090502fd3234ed25ea70a23
Author: shema-felix <shemabfelix@gmail.com>
Date:   Mon May 15 21:36:06 2023 +0200
commit 89068f285415c88050ee28da712da3a7d0dc4c90 (HEAD -> ft/team-page, origin/ft/team-page)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 19:02:42 2023 +0200

    team page commit

commit 5319a1f8e81d982974620703b356e5e01a71df18 (origin/main, main, ft/contact-page)
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Thu May 18 18:52:37 2023 +0200

    Update README.md

commit 89068f285415c88050ee28da712da3a7d0dc4c90 (HEAD -> ft/team-page, origin/ft/tea
m-page)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 19:02:42 2023 +0200

    team page commit

commit 5319a1f8e81d982974620703b356e5e01a71df18 (origin/main, main, ft/contact-page)
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Thu May 18 18:52:37 2023 +0200

    Update README.md

commit bdcb76beff61e836043eb575bcd661ff4d3bd451
Merge: 1e6144d 1a7ba88
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:49:43 2023 +0200

    Merge branch 'ft/service-redesign'

commit 1a7ba888c45dbfab7db947c22d71ef358610c802 (origin/ft/service-redesign, ft/service-redesign)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:39:43 2023 +0200

    third commit

commit 1e6144dea5f86b106c0f892ed6622cf265e4869a
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:35:29 2023 +0200

    commiting adress

commit 3d802774b017c267e2a8789d8fd88df7bce9d970
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:31:07 2023 +0200

    2nd list

commit 0a81061db6f1558af7af801f3f402483635507e1
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:20:13 2023 +0200

    unordered list

commit cc249df1760c04c5d41c8c5a4ca12ec431b8a507
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Wed May 17 19:09:18 2023 +0200

...skipping...
    third commit

commit 1e6144dea5f86b106c0f892ed6622cf265e4869a
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:35:29 2023 +0200

    commiting adress

commit 3d802774b017c267e2a8789d8fd88df7bce9d970
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:31:07 2023 +0200

    2nd list

commit 0a81061db6f1558af7af801f3f402483635507e1
Author: shema-felix <shemabfelix@gmail.com>
Date:   Wed May 17 20:20:13 2023 +0200

    unordered list

commit cc249df1760c04c5d41c8c5a4ca12ec431b8a507
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Wed May 17 19:09:18 2023 +0200

    Update README.md

commit b35f9075b375e6968e0f87bb6cd7a30fb1a7c8f6
commit 89068f285415c88050ee28da712da3a7d0dc4c90 (HEAD -> ft/team-page, origin/ft/team-page)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 19:02:42 2023 +0200

    team page commit

commit 5319a1f8e81d982974620703b356e5e01a71df18 (origin/main, main, ft/contact-page)
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Thu May 18 18:52:37 2023 +0200

    Update README.md

commit bdcb76beff61e836043eb575bcd661ff4d3bd451
Merge: 1e6144d 1a7ba88
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:49:43 2023 +0200

    Merge branch 'ft/service-redesign'

commit 1a7ba888c45dbfab7db947c22d71ef358610c802 (origin/ft/service-redesign, ft/service-redesign)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:39:43 2023 +0200


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git log
commit 89068f285415c88050ee28da712da3a7d0dc4c90 (HEAD -> ft/team-page, origin/ft/team-page)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 19:02:42 2023 +0200

    team page commit

commit 5319a1f8e81d982974620703b356e5e01a71df18 (origin/main, main, ft/contact-page)
Author: SHEMA BUGINGO FELIX <131344775+shema-felix@users.noreply.github.com>        
Date:   Thu May 18 18:52:37 2023 +0200

    Update README.md

commit bdcb76beff61e836043eb575bcd661ff4d3bd451
Merge: 1e6144d 1a7ba88
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:49:43 2023 +0200

    Merge branch 'ft/service-redesign'

commit 1a7ba888c45dbfab7db947c22d71ef358610c802 (origin/ft/service-redesign, ft/service-redesign)
Author: shema-felix <shemabfelix@gmail.com>
Date:   Thu May 18 18:39:43 2023 +0200

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/contact-page)
$ git cherry-pick 1a7ba888c45dbfab7db947c22d71ef358610c802
[ft/contact-page acf70d2] third commit
 Date: Thu May 18 18:39:43 2023 +0200
 1 file changed, 8 insertions(+), 1 deletion(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/contact-page)
$ git status
On branch ft/contact-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

[ft/contact-page c86834e] fourth commit
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 663 bytes | 221.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/shema-felix/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/contact-page)
$ git switch -c ft/faq-page
$ git commit -m "fifth commit on faq"
[ft/faq-page 585fc31] fifth commit on faq
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git revert 1a7ba888c45dbfab7db947c22d71ef358610c802
[ft/faq-page 1958d1e] Revert "third commit"
 1 file changed, 1 insertion(+), 8 deletions(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git revert 89068f285415c88050ee28da712da3a7d0dc4c90
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
error: could not revert 89068f2... team page commit
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page|REVERTING)
$ git revert 1a7ba888c45dbfab7db947c22d71ef358610c802
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
You are currently reverting commit 89068f2.
  (fix conflicts and run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page|REVERTING)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page|REVERTING)
$ git revert 1a7ba888c45dbfab7db947c22d71ef358610c802
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page|REVERTING)
$ git stash
Saved working directory and index state WIP on ft/faq-page: 1958d1e Revert "third commit"

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git revert 1a7ba888c45dbfab7db947c22d71ef358610c802
On branch ft/faq-page
nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git status
On branch ft/faq-page
nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 669 bytes | 669.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/shema-felix/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$
  #####
  #bundle 3
  
  #exercise2
  
  
HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/faq-page)
$ git switch -c ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git switch main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git pull
Updating 5319a1f..e796447
Fast-forward
 README.md     | 453 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 services.html |   9 +-
 team.html     |   2 +-
 3 files changed, 462 insertions(+), 2 deletions(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)        

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git rebase main
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   faq.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git commit -m "sixth commit"
[ft/home-page-redesign 9d5fe91] sixth commit
 1 file changed, 1 insertion(+)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git rebase main
Current branch ft/home-page-redesign is up to date.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git add .

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   home.html


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git commit -m "7th commit after rebase"
[ft/home-page-redesign 5c99a28] 7th commit after rebase
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (12/12), 1.16 KiB | 396.00 KiB/s, done.
Total 12 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:    
remote:      https://github.com/shema-felix/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/shema-felix/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

HP@DESKTOP-3RRG9G3 MINGW64 ~/Desktop/gym (ft/home-page-redesign)
$
  #####
