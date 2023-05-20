# GIT EXERCISES

## BUNDLE1

### EXERCISE1

```bash
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git init                 
Initialized empty Git repository in C:/Users/AAA/Desktop/Gym Git Exercise Solutions/.git/
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -m master main
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "first commit"
[main (root-commit) a8a68b7] first commit
 3 files changed, 198 insertions(+)      
 create mode 100644 README.md
 create mode 100644 gitexercises.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git       
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking

Enumerating objects: 5, done.
Delta compression using up to 4 threads
Writing objects: 100% (5/5), 2.54 KiB | 867.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout -b dev                                                                        
Switched to a new branch 'dev'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout -b test                                                                       
Switched to a new branch 'test'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout dev                                                                           
Switched to branch 'dev'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -D test                                                                         
Deleted branch test (was a8a68b7).



PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash
No local changes to save
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add home.html
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Untracked files:

Saved working directory and index state WIP on dev: a8a68b7 first commit
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status
  (use "git add <file>..." to include in what will be committed)

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add about.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status        
On branch dev
nothing to commit, working tree clean
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add team.html 
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash        
Saved working directory and index state WIP on dev: a8a68b7 first commit
stash@{0}: WIP on dev: a8a68b7 first commit
stash@{1}: WIP on dev: a8a68b7 first commit
stash@{2}: WIP on dev: a8a68b7 first commit
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash pop 2
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{2} (507b3ad3099748b12a1a5085c80445d6ec8709e4)
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash list
stash@{0}: WIP on dev: a8a68b7 first commit
stash@{1}: WIP on dev: a8a68b7 first commit
stash@{2}: WIP on dev: a8a68b7 first commit
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html
Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)

PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
[dev bb8a32b] second commit
 create mode 100644 home.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
error: remote origin already exists.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -D test
error: Cannot delete branch 'test' checked out at 'C:/Users/AAA/Desktop/Gym Git Exercise Solutions'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout dev
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -D test
Deleted branch test (was bb8a32b).
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions>   git push --set-upstream origin dev
Enumerating objects: 6, done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:
To https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash list
stash@{0}: WIP on dev: a8a68b7 first commit
stash@{1}: WIP on dev: a8a68b7 first commit
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add team.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add about.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash pop 1
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped refs/stash@{1} (8b8126b7770261f149489f0e3a3ee59f8c49495b)
stash@{0}: WIP on dev: a8a68b7 first commit
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git stash pop 0
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped refs/stash@{0} (ca0499cfa96fc6bbde324f64b70b3b26eb4b19eb)
commit bb8a32bed709b49c98c30d277ec5a089bb3d3be6 (HEAD -> dev, origin/dev)
Author: mutonirachel <109520133+mutonirachel@users.noreply.github.com>
Date:   Sun May 14 17:47:54 2023 +0200

    second commit

commit a8a68b764b88f2a09b8ce9f4887de010b9abcf69 (origin/main, main)
Author: mutonirachel <109520133+mutonirachel@users.noreply.github.com>
Date:   Sun May 14 17:11:21 2023 +0200

    first commit
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git reset --hard bb8a32bed709b49c98c30d277ec5a089bb3d3be6
HEAD is now at bb8a32b second commit
```
## BUNDLE2

### EXERCISE1

```bash
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)    
        modified:   README.md

Untracked files:
        service.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add sercvise.html  
fatal: pathspec 'sercvise.html' did not match any files
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add sercvce.html   
fatal: pathspec 'sercvce.html' did not match any files
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add sercvice.html  
fatal: pathspec 'sercvice.html' did not match any files
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add service.html   
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "another 
commit"
[ft/bundle-2 425e87b] another commit
 1 file changed, 12 insertions(+)
 create mode 100644 service.html
 PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "changes on service file to be committed"
[ft/service-design 6b01f88] changes on service file to be committed
 2 files changed, 215 insertions(+)
 create mode 100644 service.html
fatal: The current branch ft/service-design has no upstream branch.
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin ft/service-design

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push --set-upstream origin ft/service-design
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 2.36 KiB | 604.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/service-design' on GitHub by visiting:
remote:      https://github.com/mutonirachel/Gym-Git-Exercise-Solutions/pull/new/ft/service-design
remote:
To https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-design -> ft/service-design
branch 'ft/service-design' set up to track 'origin/ft/service-design'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout ft/service-design
Already on 'ft/service-design'
Your branch is up to date with 'origin/ft/service-design'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git mergre main
git: 'mergre' is not a git command. See 'git --help'.

The most similar command is
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add service.html                                     
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "other changes on service file"
[main 492907a] other changes on service file
 1 file changed, 13 insertions(+)
 create mode 100644 service.html
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 510 bytes | 102.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
   a8a68b7..492907a  main -> main
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git checkout ft/service-design
Switched to branch 'ft/service-design'
Your branch is up to date with 'origin/ft/service-design'.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git diff main..ft/service-design 
diff --git a/README.md b/README.md
index e69de29..120b45a 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1,202 @@
+# GIT EXERCISES
+
+## BUNDLE1
+
+### EXERCISE1
+
+```bash
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git init
+Initialized empty Git repository in C:/Users/AAA/Desktop/Gym Git Exercise Solutions/.git/
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -m master main
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "first commit"
+[main (root-commit) a8a68b7] first commit
+ 3 files changed, 198 insertions(+)
+ create mode 100644 README.md
+ create mode 100644 gitexercises.html
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gy:...skipping...
diff --git a/README.md b/README.md
index e69de29..120b45a 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1,202 @@
+# GIT EXERCISES
+
+## BUNDLE1
+
+### EXERCISE1
+
+```bash
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git init
+Initialized empty Git repository in C:/Users/AAA/Desktop/Gym Git Exercise Solutions/.git/
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -m master main
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "first commit"
+[main (root-commit) a8a68b7] first commit
+ 3 files changed, 198 insertions(+)
+ create mode 100644 README.md
+ create mode 100644 gitexercises.html
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
:...skipping...
diff --git a/README.md b/README.md
index e69de29..120b45a 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1,202 @@
+# GIT EXERCISES
+
+## BUNDLE1
+
+### EXERCISE1
+
+```bash
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git init
+Initialized empty Git repository in C:/Users/AAA/Desktop/Gym Git Exercise Solutions/.git/
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -m master main
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "first commit"
+[main (root-commit) a8a68b7] first commit
+ 3 files changed, 198 insertions(+)
+ create mode 100644 README.md
+ create mode 100644 gitexercises.html
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
+fatal: The current branch main has no upstream branch.
+To push the current branch and set the remote as upstream, use
+
+    git push --set-upstream origin main
+
:...skipping...
diff --git a/README.md b/README.md
index e69de29..120b45a 100644     
diff --git a/README.md b/README.md
index e69de29..120b45a 100644
diff --git a/README.md b/README.md
index e69de29..120b45a 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1,202 @@
+# GIT EXERCISES
+
+## BUNDLE1
+
+### EXERCISE1
+
+```bash
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git init
+Initialized empty Git repository in C:/Users/AAA/Desktop/Gym Git Exercise Solutions/.git/
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git branch -m master main
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git add .
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "first commit"
+[main (root-commit) a8a68b7] first commit
+ 3 files changed, 198 insertions(+)      
+ create mode 100644 README.md
+ create mode 100644 gitexercises.html
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git remote add origin https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git       
+PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
+fatal: The current branch main has no upstream branch.
+To push the current branch and set the remote as upstream, use
+
+    git push --set-upstream origin main
+
+To have this happen automatically for branches without a tracking
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git merge main
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git status
>> q'
>> "^C
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git commit -m "last changes"
[ft/service-design a9be228] last changes
PS C:\Users\AAA\Desktop\Gym Git Exercise Solutions> git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 288 bytes | 288.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/mutonirachel/Gym-Git-Exercise-Solutions.git
   6b01f88..a9be228  ft/service-design -> ft/service-design
 ```