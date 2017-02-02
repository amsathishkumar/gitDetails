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
-------------------------------------
    git diff >> sat.diff
    patch < sat.diff
