1. git initialization
$ git config --global user.name "yourname"
$ git config --global user.email "youremail"
$ git config --global init.defaultBranch main

2. Create .git folder for project initial
$ git init

3. Check the repository change and commit
$ git status // Check the repository change
$ git add . //Add all changed file
$ git commit -m "your commit" //commit

4. Back to the past
4-1 reset
$ git log //Check the commit log 
$ git reset --hard (commit hash)

4-2 revert
$ git revert (commit hash)

$ git revert --no-commit (commit hash) // If you want not commit at revert
$ git reset --hard // If you want cancel the revert

5. branch
$ git branch (branch name)// Create branch
$ git branch // Check brach list
$ git switch (branch name) // move to branch name
$ git branch -d (branch name) // delete branch
$ git branch -m (current branch name) (new branch name) // Change branch name

6. merge
$ git merge (branch name)

7. github
$ git remote add origin (repository address)
$ git branch -M main
$ git push -u origin main

8. push & pull
$ git push
$ git pull

// If you do push before pull 
$ git pull --no-rebase // merge
$ git pull --rebase // rebase

9. remote branch
$ git push -u origin (branch name) // Create and Connect remote branch to local branch

// Get remote branch to local
$ git fetch
$ git switch -t origin/(branch name)

$ git push origin --delete (remote branch)// delete remote branch
$ git remote prune origin // update remote branch
