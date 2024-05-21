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
