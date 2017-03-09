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

Git Version:
-------------------------------------
     #TAG=$(git --git-dir=/root/sat/.git describe --abbrev=0 --tags )
     #echo $TAG
     v6.2
     
     #VER=$(echo $TAG.$(git --git-dir=/root/sat/.git log $TAG.. --oneline | wc -l ) | sed 's/[^0-9.]//g')
     #echo $VER
     6.2.999
     
     #REL=$(git --git-dir=/root/sat/.git rev-parse --short HEAD)
     #echo $REL
     8e70122 <commit id>

Git TAG Delete
-----------------------------------
	#git tag 
        staging-sat
    #git tag -d staging-sat
    #git push origin :refs/tags/staging-sat
    
Git TAG Add
----------------------------------
    #git tag -a  staging-sat <commit id>
    #git push origin staging-sat

GIT to create branch and push
----------------------------------
	git checkout -b sat-1705
	git commit -m "sat-1705changes"
	git push origin sat-1705

Delete local changes
----------------------------------
	git clean -f -d
