### gitExercise2

## Part 1

```
ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 8fae7631f217911a02944d0c779ad4ac70733c2a (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit b291a72408e1930e43124c031c5e25e0b9338e0d
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create another file

commit 1438792869560a2da326bacbdab0e933984f2789
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create initial file

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git add test4.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git commit --amend --no-edit
[main de09fdb] chore: Create third and fourth files
 Date: Tue May 21 12:25:58 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md

 ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git rebase -i HEAD~2
[detached HEAD 971a241] chore: Create second file
 Date: Tue May 21 12:25:57 2024 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 285f7adc918b6746722302de4f21b30782cc1019 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit 971a2418f40b6666e004a32d0271f1654a119262
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create second file

commit 1438792869560a2da326bacbdab0e933984f2789
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create initial file
    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 285f7adc918b6746722302de4f21b30782cc1019 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit 971a2418f40b6666e004a32d0271f1654a119262
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create second file

commit 1438792869560a2da326bacbdab0e933984f2789
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create initial file

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git rebase -i --root
[detached HEAD 8248c41] chore: create the first two files
 Date: Tue May 21 12:25:57 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 443af88ee6445dfbdea1c18c748ef9649c699931 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit 8248c4197a22a90026987236bbd3c6a7cd55a5f4
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 443af88ee6445dfbdea1c18c748ef9649c699931 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit 8248c4197a22a90026987236bbd3c6a7cd55a5f4
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git rebase -i Head~1
Stopped at 443af88...  chore: Create third and fourth files
You can amend the commit now, with

  git commit --amend

Once you are satisfied with your changes, run

  git rebase --continue

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git status
interactive rebase in progress; onto 8248c41
Last command done (1 command done):
   edit 443af88 chore: Create third and fourth files
No commands remaining.
You are currently editing a commit while rebasing branch 'main' on '8248c41'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git reset HEAD~

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git status
interactive rebase in progress; onto 8248c41
Last command done (1 command done):
   edit 443af88 chore: Create third and fourth files
No commands remaining.
You are currently editing a commit while rebasing branch 'main' on '8248c41'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test3.md
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git add test3.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git commit -m"create third file"
[detached HEAD 5b3e6ea] create third file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git add test4.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git commit -m"create fourth file"
[detached HEAD 70851ec] create fourth file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|REBASE 1/1)
$ git rebase --continue
Successfully rebased and updated refs/heads/main.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 945d29e56f70f52cd5405ebccc043974c803c512 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:19:33 2024 +0200
pick 0a42925 create third and fourth files

    Unwanted commit

commit 0a4292517dc5890e0f987be44bfb5303ef1af7a5
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 13:49:08 2024 +0200

    create third and fourth files

    create fourth file

commit 8248c4197a22a90026987236bbd3c6a7cd55a5f4
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git rebase -i Head~2
Successfully rebased and updated refs/heads/main.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 0a4292517dc5890e0f987be44bfb5303ef1af7a5 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 13:49:08 2024 +0200

    create third and fourth files

    create fourth file

commit 8248c4197a22a90026987236bbd3c6a7cd55a5f4
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git rebase -i --root
Successfully rebased and updated refs/heads/main.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit 077b3f71f611969c6f3d8ab2e0094e12ca73c0be (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

commit c305411b3a13778fb255b5b5f1f59002c7cca303
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 13:49:08 2024 +0200

    create third and fourth files

    create fourth file

    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git checkout -b ft/branch
Switched to a new branch 'ft/branch'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/branch)
$ git add .

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/branch)
$  git commit -m"Implemented test 5"
[ft/branch 6c1ac40] Implemented test 5
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/branch)
$ git log
commit 6c1ac400dce5dd24ae1bbc8fba2eb408b1ba6630 (HEAD -> ft/branch)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:50:39 2024 +0200

    Implemented test 5

commit 077b3f71f611969c6f3d8ab2e0094e12ca73c0be (main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

:...skipping...
commit 6c1ac400dce5dd24ae1bbc8fba2eb408b1ba6630 (HEAD -> ft/branch)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:50:39 2024 +0200

    Implemented test 5

commit 077b3f71f611969c6f3d8ab2e0094e12ca73c0be (main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

commit c305411b3a13778fb255b5b5f1f59002c7cca303
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 13:49:08 2024 +0200

    create third and fourth files

    create fourth file

    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/branch)
$ git checkout main
Switched to branch 'main'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git cherry-pick 6c1ac400dce5dd24ae1bbc8fba2eb408b1ba6630
[main ff82239] Implemented test 5
 Date: Tue May 21 14:50:39 2024 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log
commit ff82239d7eb3bc4cb31c596567d84fce4031b4e0 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:50:39 2024 +0200

    Implemented test 5

commit 077b3f71f611969c6f3d8ab2e0094e12ca73c0be
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: create the first two files

    chore: Create initial file

    chore: Create second file

commit c305411b3a13778fb255b5b5f1f59002c7cca303
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 13:49:08 2024 +0200

    create third and fourth files

    create fourth file

    ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git log --graph
* commit ff82239d7eb3bc4cb31c596567d84fce4031b4e0 (HEAD -> main)
| Author: DevRamona <r.ingabire@alustudent.com>
| Date:   Tue May 21 14:50:39 2024 +0200
| 
|     Implemented test 5
| 
* commit 077b3f71f611969c6f3d8ab2e0094e12ca73c0be
| Author: DevRamona <r.ingabire@alustudent.com>
| Date:   Tue May 21 12:25:57 2024 +0200
| 
|     chore: create the first two files
|     
|     chore: Create initial file
|     
|     chore: Create second file
| 
* commit c305411b3a13778fb255b5b5f1f59002c7cca303
  Author: DevRamona <r.ingabire@alustudent.com>
  Date:   Tue May 21 13:49:08 2024 +0200
  
      create third and fourth files
      
      create fourth file

      ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git checkout -b ft/new-feature
Switched to a new branch 'ft/new-feature'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ 

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ git add .

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ git commit -m"chore: Implemented core functionality for new feature"
[ft/new-feature 37ff11f] chore: Implemented core functionality for new feature
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ 


```

## Part 2 

```
ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git checkout -b ft/new-feature
Switched to a new branch 'ft/new-feature'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ vi feature.txt

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ git add feature.txt
warning: in the working copy of 'feature.txt', LF will be replaced by CRLF the next time Git touches it

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-fe
There are introductory concepts that are added in this file
ature)
$ git commit -m "Implemented core functionality for new feature"
[ft/new-feature 3201ab4] Implemented core functionality for new feature
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-feature)
$ git switch main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ vi readme.txt

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "Updated project readme"
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add readme.text
fatal: pathspec 'readme.text' did not match any files

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "Updated project readme"
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add readme.txt
warning: in the working copy of 'readme.txt', LF will be replaced by CRLF the next time Git touches it

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "Updated project readme"
[main e9a47e1] Updated project readme
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    

$ git status 
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "history "
[main 715fe82] history
 1 file changed, 74 insertions(+)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git push 
Enumerating objects: 20, done.
Counting objects: 100% (20/20), done.
Delta compression using up to 4 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (18/18), 2.76 KiB | 314.00 KiB/s, done.
Total 18 (delta 6), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (6/6), done.
To https://github.com/DevRamona/gitExercise2.git
   b4cb870..715fe82  main -> main

>>>>>>> ft/new-branch-from-commit
ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git pull
Already up to date.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ ls
'e -i HEAD~2'   readme.txt   test2.md   test4.md
 README.md      test1.md     test3.md   test5.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git branch -d ft/new-feature
error: the branch 'ft/new-feature' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D ft/new-feature'
hint: Disable this message with "git config advice.forceDeleteBranch false"

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git branch -D ft/new-feature
Deleted branch ft/new-feature (was 3201ab4).


ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "New codes were added"
[main 32fa632] New codes were added
 1 file changed, 18 insertions(+)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git log --oneline --graph
* 32fa632 (HEAD -> main) New codes were added
* 715fe82 (origin/main, origin/HEAD) history
* e9a47e1 Updated project readme
* 5d8b559 new changes added in the README
* ffa4587 Implemented test 5
* b2f6e86 chore: Create initial file
* ef13dba Create Third and Fourth File
* b4cb870 Create README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git log 
commit 32fa6324fb561b492a02c33c8819fd3f8bae7215 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:38:19 2024 +0200

    New codes were added

commit 715fe82a71d8bed4422bf4006a9b67ceb8372eab (origin/main, origin/HEAD)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 11:01:31 2024 +0200

    history

commit e9a47e121c0b81c47a53612ef63376b3149eb326
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 10:46:22 2024 +0200

    Updated project readme

commit 5d8b55948e5dc237e13f8fa7b6a37d4635d3205a

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git log 
commit 32fa6324fb561b492a02c33c8819fd3f8bae7215 (HEAD -> main)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 14:38:19 2024 +0200

    New codes were added

commit 715fe82a71d8bed4422bf4006a9b67ceb8372eab (origin/main, origin/HEAD)
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 11:01:31 2024 +0200

    history

commit e9a47e121c0b81c47a53612ef63376b3149eb326
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 10:46:22 2024 +0200

    Updated project readme

commit 5d8b55948e5dc237e13f8fa7b6a37d4635d3205a
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Tue May 21 10:39:09 2024 +0200

    new changes added in the README

commit ffa458711f02f77996db3a77d9da78dc121144a3
Author: DevRamona <r.ingabire@alustudent.com>
Date:   Mon May 20 19:38:17 2024 +0200


ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git log --oneline -3
32fa632 (HEAD -> main) New codes were added
715fe82 (origin/main, origin/HEAD) history
e9a47e1 Updated project readme

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git checkout -b ft/new-branch-from-commit e9a47e1
Switched to a new branch 'ft/new-branch-from-commit'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$  git log --oneline --graph
* e9a47e1 (HEAD -> ft/new-branch-from-commit) Updated project readme
* 5d8b559 new changes added in the README
* ffa4587 Implemented test 5
* b2f6e86 chore: Create initial file
* ef13dba Create Third and Fourth File
* b4cb870 Create README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$
>>>>>>> ft/new-branch-from-commit


git checkout main 
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git commit -m "new"
[ft/new-branch-from-commit 0d7f486] new
 1 file changed, 237 insertions(+)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git pull origin main 
From https://github.com/DevRamona/gitExercise2
 * branch            main       -> FETCH_HEAD
Already up to date.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git merge ft/new-branch-from-commit
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|MERGING)
$ git add README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|MERGING)
$ git commit -m 'Resolved the conflict'
[main e2bebd7] Resolved the conflict

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$
ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "updated the README"
[main 39de8bf] updated the README
 1 file changed, 40 insertions(+)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git checkout ft/new-branch-from-commit
Switched to branch 'ft/new-branch-from-commit'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git pull origin ft/new-branch-from-commit
fatal: couldn't find remote ref ft/new-branch-from-commit

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git rebase main
Successfully rebased and updated refs/heads/ft/new-branch-from-commit.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git add README.md 

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git rebase --continue
fatal: No rebase in progress?

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git push origin ft/new-branch-from-commit
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 3.37 KiB | 575.00 KiB/s, done.
Total 12 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (7/7), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/new-branch-from-commit' on GitHub by visiting: 
remote:      https://github.com/DevRamona/gitExercise2/pull/new/ft/new-branch-from-commit
remote:
To https://github.com/DevRamona/gitExercise2.git
 * [new branch]      ft/new-branch-from-commit -> ft/new-branch-from-commit

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/new-branch-from-commit)
$ git branch -m ft/new-branch-from-commit ft/improved-branch-name

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/improved-branch-name)
$ git log -- oneline 

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/improved-branch-name)
$ git log --oneline --graph
* 39de8bf (HEAD -> ft/improved-branch-name, origin/ft/new-branch-from-commit, main) updated the README
*   e2bebd7 Resolved the conflict
|\
| * 0d7f486 new
* | 32fa632 New codes were added
* | 715fe82 (origin/main, origin/HEAD) history
|/
* e9a47e1 Updated project readme
* 5d8b559 new changes added in the README
* ffa4587 Implemented test 5
* b2f6e86 chore: Create initial file
* ef13dba Create Third and Fourth File
* b4cb870 Create README.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (ft/improved-branch-name)
$ git checkout e2bebd7
Note: switching to 'e2bebd7'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at e2bebd7 Resolved the conflict

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 ((e2bebd7...))
$ git checkout main 
Previous HEAD position was e2bebd7 Resolved the conflict
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$
```


## Part 3

```
ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git stash
No local changes to save

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git stash pop
No stash entries found.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git checkout -b feature-branch
Switched to a new branch 'feature-branch'

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (feature-branch)
$ vi test6.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (feature-branch)
$ git add test6.md 
warning: in the working copy of 'test6.md', LF will be replaced by CRLF the next time Git touches it

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (feature-branch)
$ git commit -m "Created the sixth file"
[feature-branch cd83825] Created the sixth file
 1 file changed, 1 insertion(+)
New additional texts
 create mode 100644 test6.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (feature-branch)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ ls
'e -i HEAD~2'   readme.txt   test2.md   test4.md
 README.md      test1.md     test3.md   test5.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ vi test6.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test6.md

nothing added to commit but untracked files present (use "git add" to track)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add test6.md 
warning: in the working copy of 'test6.md', LF will be replaced by CRLF the next time Git touches it

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "Done with the sixth"
[main a1f8a4d] Done with the sixth
 1 file changed, 2 insertions(+)
 create mode 100644 test6.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git merge feature-branch 
Auto-merging test6.md
CONFLICT (add/add): Merge conflict in test6.md
Automatic merge failed; fix conflicts and then commit the result.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|MERGING)
$ git add test6.md

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main|MERGING)
$ git commit -m "conflicts merged"
[main fc48346] conflicts merged

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git mergetool --tool-help
'git mergetool --tool=<tool>' may be set to one of the following:
                vimdiff          Use Vim with a custom layout (see `git help mergetool`'s `BACKEND SPECIFIC HINTS` section)
                vimdiff1         Use Vim with a 2 panes layout (LOCAL and REMOTE)
                vimdiff2         Use Vim with a 3 panes layout (LOCAL, MERGED and REMOTE)
                vimdiff3         Use Vim where only the MERGED file is shown

The following tools are valid, but not currently available:
                araxis           Use Araxis Merge (requires a graphical session)
                bc               Use Beyond Compare (requires a graphical session)
                bc3              Use Beyond Compare (requires a graphical session)
                bc4              Use Beyond Compare (requires a graphical session)
                codecompare      Use Code Compare (requires a graphical session)
                deltawalker      Use DeltaWalker (requires a graphical session)
                diffmerge        Use DiffMerge (requires a graphical session)
                diffuse          Use Diffuse (requires a graphical session)
                ecmerge          Use ECMerge (requires a graphical session)
                emerge           Use Emacs' Emerge
                examdiff         Use ExamDiff Pro (requires a graphical session)
                guiffy           Use Guiffy's Diff Tool (requires a graphical session)
                gvimdiff         Use gVim (requires a graphical session) with a custom layout (see `git help mergetool`'s `BACKEND SPECIFIC HINTS` section)
                gvimdiff1        Use gVim (requires a graphical session) with a 2 panes layout (LOCAL and REMOTE)
                gvimdiff2        Use gVim (requires a graphical session) with a 3 panes layout (LOCAL, MERGED and REMOTE)
                gvimdiff3        Use gVim (requires a graphical session) where only the MERGED file is shown
                kdiff3           Use KDiff3 (requires a graphical session)
                meld             Use Meld (requires a graphical session) with optional `auto merge` (see `git help mergetool`'s `CONFIGURATION` section)
                nvimdiff         Use Neovim with a custom layout (see `git help mergetool`'s `BACKEND SPECIFIC HINTS` section)
                nvimdiff1        Use Neovim with a 2 panes layout (LOCAL and REMOTE)
                nvimdiff2        Use Neovim with a 3 panes layout (LOCAL, MERGED and REMOTE)
                nvimdiff3        Use Neovim where only the MERGED file is shown
                opendiff         Use FileMerge (requires a graphical session)
                p4merge          Use HelixCore P4Merge (requires a graphical session)
                smerge           Use Sublime Merge (requires a graphical session)
                tkdiff           Use TkDiff (requires a graphical session)
                tortoisemerge    Use TortoiseMerge (requires a graphical session)
                winmerge         Use WinMerge (requires a graphical session)
                xxdiff           Use xxdiff (requires a graphical session)

Some of the tools listed above only work in a windowed
environment. If run in a terminal-only session, they will fail.

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$