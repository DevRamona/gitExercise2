# gitExercise2


rm -r gitExercises
   79  mkdir git_exercises
   80  cd git_exercises
   81  git init
   82  git status
   83  vi README.md
   84  rm -r README.md
   85  ls
   86  git branch -m main
   87  vi README.md
   88  ls
   89  git add README.md
   90  git commit -m "A file has been added"
   91  git remote add https://github.com/DevRamona/gitStarted.git
   92  git remote add origin https://github.com/DevRamona/gitStarted.git
   93  git push --set-upstream origin main
   94  git status
   95  git checkout b dev
   96  git checkout -b dev
   97  git status
   98  git branch
   99  git push origin dev
  100  git checkout -b test
  101  git push origin test
  102  git checkout dev
  103  git branch -d test
  104  git push origin --delete test
  105  git log --graph
<<<<<<< HEAD

  ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
=======
 git status 
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git add README.md 

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
$ git commit -m "new changes added in the README"
New feature is created to implement some functionalities
[main 5d8b559] new changes added in the README
 1 file changed, 30 insertions(+)

ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
>>>>>>> ft/new-branch-from-commit
$ git branch
  ft/branch
* main

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
<<<<<<< HEAD
=======

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