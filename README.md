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

  ingab@DESKTOP-13J8UH7 MINGW64 ~/Desktop/git-advanced-exercise/gitExercise2 (main)    
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
$
