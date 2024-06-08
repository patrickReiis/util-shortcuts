show commit: **git diff COMMIT~ COMMIT**

show commit but not merges: **git show COMMIT**

goes back a commit: **git reset HEAD^**

------ start how to rebase

**git checkout feature-branch**

**git rebase -i master**

**git checkout master**

**git merge feature-branch**

------ end how to rebase


------ start PUSH TO REMOTE BRANCH // OPEN MERGE REQUEST
```
git checkout -B <123-branch>  
// do some changes  
git add src/*  
git commit -m "feat: hi"  
***git push -u origin <123.branch>***
```
------ end PUSH TO REMOTE BRANCH // OPEN MERGE REQUEST  

------ start PUSH COMMIT TO OPEN MERGE REQUEST YOU DID NOT CREATE
```
git fetch
git checkout origin/<my-branch>
// do some changes  
git add src/*  
git commit -m "feat: hi"  
***git push origin HEAD:<branch-name>***
```
------ end PUSH TO REMOTE BRANCH // OPEN MERGE REQUEST  

