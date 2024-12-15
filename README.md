# git-training

1034  git clone https://github.com/manhhad32/git-training.git 
1035  cd git-training
1036  git status
1037  git branch
1038  git checkout dev
1039  git fetch
1040  git checkout dev
1041  git branch


+ commit 2 (14b79ca8c3)
+ commit 1 (14b79ca8c6)
+ commit a (14b79ca8c7)

combine multi commits (commit 2 + commit 1)
git reset --soft 14b79ca8c7
git merge --squash
git commit -a -m"task a" 
git push --force.

---
resole conflict
--- branch features/task-a (confict code)
git checkout dev 
git pull
git checkout -b dev-resolve-conflict
git push --set-upstream dev-resolve-conflict
git merge features/task-a
-- use git tool in editor to resolve conflict code.
git commit -a -m"resolved conflict task-a"
git push
-----
create pull request dev-resolve-conflict ----> dev
