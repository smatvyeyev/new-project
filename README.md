# How to create git repo with "development" branch.
#

 Create project directory  -  % mkdir new-project
 Go to the directory - % cd new-project 
 Create GIT repo - new-project % git init
 Check status - new-project % git status
 Add readme file - new-project % touch README.md

 Add info to README.md file with any situable editor. (VI, VIM, NANO etc.)

 Add README.md file to tracking and commit to repo:
       new-project % git add README.md 
       new-project % git commit -m "init"

 Create a repo branch 'development' - new-project % git checkout -b development
 # Note that the git status command tells you which branch you are on.

 For switching to the brach use - new-project % git checkout <branche name> | i.e. % git checkout main
 Listing of your current branches - new-project % git branch

 Add new info to README.md file with any situable editor. (VI, VIM, NANO etc.)
 save changes:
       new-project % git add README.md 
       new-project % git commit -m "Added to README file"

 To merge development branch with main branch (brings changes from two branches into one)
 run commands:
       new-project % git checkout development 
       new-project % git merge main 

 Yuo can check successfulymerged branches by run:
       new-project % git branch --merged 
