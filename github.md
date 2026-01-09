git config --global user.name ""

git config --global user.email ""

git config --global core.editor "code --wait"

git config --global core.autocrlf "input"

git config --global -e --> edit the configuration of user

git log --oneline --> log saved checkpoint

git reset --hard HEAD~1 --> Back checkpoint

git status -s --> check status of file track of file

git status --> file changes status and state before and after commit of file status

git log --> history commited

rm .git --> remove a git

git branch branch_name --> create a branch

git branch --> check a how many branch

git switch branchName --> change a branch

git branch -d branchName --> Delete Branch

git switch -C branchName --> create branch and switch brnch

--> merge branch == switch into main branch

git merge branchName

git stash --> chnages not commited and switch to another branch

git stash apply --> back to branch and apply old changes return


git clone link --> repository clone of project








//collab

--> Main -> Computer
-->Developer -> Het

->computer create initial code and create repo amd innital code push on github 

-> github in provide a user access

-> het clone the project 
-> create branch
 -> add code
 -> git add . 
 -> git commit -m ""
 -> git push -u origin branchName


-> computer 
>git fetch
>git branch 
>git switch branchName
>git switch main
> git merge BranchnName
>git push origin main

//computer push code on github main branch
// het fetch the code of main branch 
>git switch main
> git fetch
> git pull