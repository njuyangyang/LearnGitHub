# Learn GitHub

This document is to teach your how to set **upstream** for the course project. Briefly, every one fork this repo to your own github. and then mirrow to your local or Cloud9. Make changes, merge your code with the updated project in your local and then request pulls.

## Todo list
 - fork this repo
 - clone to your local or cloud9
 - make change at the end of this document
 - fectch the updated upstream
 - merge in the local
 - push to your own remote repo
 - pull request.

## The commands your will use
```sh
 $git clone git@github.com:[username]/LearnGitHub.git
 ```
 
 Now, you can check your remote in your local
  ```sh
  $git remote
  origin
  ```
  After your work, your want to merge the your work to my main repo. However, maybe my repo has changed during this period. You should get my refreshed my code and make it work in your local. And then send the pull request, which will obviously reduces the maintainer's work load.
  
  To do so, you should firstly **fetch**  the updated code from my repo to your local rather from your own repo. so you need set my repo as your **upstream**.
  
  ```sh
  $git add remote upstream git@github.com:njuyangyang/LearnGitHub.git
  ```
  
  now you can check your remote again.
  ```sh
  $git remote
  upstream
  origin
  ```
  
  to see more details
  ```sh
$git remote -v
origin	git@github.com:njuyangyang/LearnGitHub.git (fetch)
origin	git@github.com:njuyangyang/LearnGitHub.git (push)
  ```
  
  ## After your work
  you should fetch my code from upstream.
  
  ```sh
  $git fetch upstream
  ```
  
  After the **fetch**, you should try to merge it with your code firstly.
  
  ```sh
  git merge upstream/master
  ```
  
  If some problem happend. your should change fix the conflicts firstly in your local. 
  
  Woshimeinv
  ```sh
  $git diff [path1] [path2]
  ```
## now you can push it to your repo and then pull request!!!!

### Try change