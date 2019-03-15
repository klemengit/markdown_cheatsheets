# GitHub basic instructions

Some instructions from: https://www.howtoforge.com/tutorial/install-git-and-github-on-ubuntu-14.04/


## SET UP GIT:
* Install Git:
  ```
  sudo apt-get install git
  ```

* Configure GitHub:
  ```
  git config --global user.name "user_name"
  git config --global user.email "email_id"
  ```

## CREATE REPOSITORY:
* Local repositoriy:
  ```
  git init repository_name
  cd repository_name
  ```

* Create repository on GitHub:
  * go to web-site and create repository
  * copy the URL
  ```
  git remote add origin https:... (URL of repository)
  ```

## WORK IN REPOSITORY:
* Add repository files to index:
  ```
  git add README
  git add all_files_that_you_have_created or git add .
  ```

* Commit changes:
  ```
  git commit -m "message"
  ```

* Push files to GitHub repository:
  ```
  git push origin master/name_of_branch
  ```

* Pull from GitHub:
  ```
  git pull origin master (or a branch)
  ```

* Create a new branch:
  ```
  git checkout -b name_of_branch
  ```

* Commit changes on branch:
  ```
  git commit -m "message"
  ```

* Switch between branches or branch and master:
  ```
  git checkout name_of_branch_you_want_to_switch_to
  ```
  
* Merge branch with master:
  ```
  git checkout master
  git merge name_of_branch
  ```
  
* Delete branch that you don't need anymore:
  ```
  git branch -d name_of_branch
  ```

* Delete directory:
  ```
  git rm -r directory_name
  ```

