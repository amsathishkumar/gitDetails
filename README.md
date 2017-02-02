# gitDetails

To find modified details:
-------------------------------------
    git diff HEAD file.txt


Create Branch and commit
-------------------------------------
    git checkout -b branchname
    git commit -m "branchname changes"
    git push origin branchname

Git Branch
-------------------------------------
    git branch
    git branch –a  local branches
    git branch –r  remote branches
    git remote 
    git ls-remote
    Switch to branch: git checkout branchname


Import git diff (make sure branch are same)
-------------------------------------------
    git diff >> sat.diff
    patch < sat.diff

if the commit only exists in your local repository (Index/Unstage)and has not been pushed to GitHub, you can amend the commit message with the
-------------------------------------
    git commit --amend
