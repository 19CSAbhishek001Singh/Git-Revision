1. `git init` ->Powers your folder to be managed  by git, and inititalize a new empty repo. It
also create a .git folder that has all the relevant logic to manage versions of your project. 

2. `Working Area` -> there can be bunch of files that are not currently handled by git.
means that changes done or to be done in those files are not managed by git yet. When we
do `git status` we see bunch of untarcked files then these are in working area.

3. `Staging area` -> what all files are going to be part of next version that we will create.
it is the place where git knows what chnages will be done from the last version to the next version.

4. `Repository area` -> This area actually contains the details of all your previous registered version.
And all the files in this area, git already manages them and knows their version.

5. `git add <file> -> moves file from working area to stage area

6. `git rm --cached <file>` -> moves file back from staging to working area

7. `commit -> commit is a particular version of the project. It captures a snapshot of the project's staged
changes and creates a version out of it.

8. `git commit` -> register staging chnages toa commit means techinal now in Repository area.

9. `git log` -> list down all the commits of the Repository.

10. `git restore <file>` -> to discard changes in working directory now git is tracking so techincally commited chnagesare in staging are
and new things in working area.If we did some bad code we can we can use this, instead of deleting every change line by line or say go to
 last version.

11. `git restore --staged <file>` -> to unstage,it remove file from chnages from staging to working area.
this work only chnages are in staging area.

12. differnce b/w git rm and git restore 
if you want to  move the whole file back to the untracked status we do git rm otherwise if we just wanted chnages to be 
moved in working or staging area then git restore
can't to git rm if we have staging chnages.

13. `git diff commit1 commit2`-> gives differnce of files between two commits

14. 'git commit -m "mesage"` -> to not open vim directly provide commit messages do this.

15. `git remote`-> list down all the remote connection names

16. Remote connections -> lik two git repo for uploading and dowloading changes from each otherwise

17. `git remote add <name of remote> <link of repo> -> this help us to add a new link to the remote and give a name to it

18. `git remote rm <name of remote>` -> to delete a remote connection

19. `git remote rename <old name> <new name>` -> this command renames the remote connection

remote name is always used to establish connection