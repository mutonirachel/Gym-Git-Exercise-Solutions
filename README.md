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
```