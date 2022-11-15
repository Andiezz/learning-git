# git command

## basic commands

### `git status`
    - Show the files and changes that have not tracked (# committed)  yet.

### `git add / git add .`
    - Tell git which file to track (ready to commit)

### `git commit -m "<name>" -m <message>`
    - Commit changes to the local repo

### `git commit -am -m <message>`
    - Add and commit (just with old files)

### `git push / git push origin master` 
    - Push the local repo to remote repo

### SSH keys
    - To prove to GitHub you are the owner of your account
    - Connect the local machine to the GitHub
#### `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
    - id_rsa: private key
    - id_rsa.pub: public key
#### Adding connection to the local github
    - in Git Bash
##### `eval "$(ssh-agent -s)"`
    - Start the ssh-agent in the background
##### `ssh-add ~/.ssh/<your_key_name>`
    - Add your SSH private key to the ssh-agent.

### `git init`
    - Initialize git repo

### `git remote add origin`
    - Add the reference to the remote repo

### `git remote -v`
    - Check the version of git remote

### `git push -u origin master`
    - Set default where to push, after that just `git push`


## git branching

### `git branch`
    - Check the branches

### `git checkout -b <name of feature branch>`
    - Create a new branch

### `git checkout`
    - Switch between branches

### `git diff <branch name>`
    - Check the changes in the other branch

### `git push --set-upstream origin feature-branch-2`
    - Push the branch to the remote repo to merge by GitHub
    - And then create a *Pull Request*

### `git branch -d <feature-branch>`
    - Delete the branch

### `git reset nothing/<filename>`
    - Undo tracking / staging (not add yet)

### `git reset HEAD~(number of commit you want to undo)` / `git reset <hash code of commit>`
    - HEAD pointer to last commit

### `git reset --hard <hash code of commit>`
    - Change directly
