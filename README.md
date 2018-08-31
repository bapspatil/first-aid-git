
# first-aid-git

A quick guide and list of commands related to Git & GitHub.
<br>If you're new to Git and GitHub or want to deepen your knowledge about it, this repository is for you.

**Feel free to email any doubts you may have at <a href="mailto://hi@bapspatil.com">hi@bapspatil.com</a>.**

## Here you go:

* Configuring the username in Git

    `git config --global user.name "Firstname Lastname"`

    * To display the username set

        `git config --global user.name`

* Configuring email in Git

    `git config --global user.email "youremail@example.com"`

    * To display the email set

        `git config --global user.email`

* Create a new local Git repository

    `git init`

* Add files for commit

    * To add all files in the current folder/directory

        `git add .`

    * To add a single file

        `git add <file-name>`

    * To add multiple files

        `git add <file-1> <file-2>`

* Commiting files

   `git commit -m "Descriptive commit message"`

* Adding a remote, i.e. the GitHub URL for your repository

    `git remote add origin <repository-url>.git`

* Push - Update changes to repository on GitHub

    * To push to `master` branch
  
        `git push -u origin master`

    * To force-push (**Warning**: This erases all previous commits)

        `git push -u origin master -f`

    * To push to a different branch
  
        `git push -u origin <branch-name>`

* Clone a repository

   `git clone <repository-url>`

* Create a new branch from current working branch and switch to it

   `git checkout -b <new-branch-name>`

* Create new branch from an existing branch and stay in the current branch

    `git checkout -b <new-branch> <existing-branch>`

* Switch to a new branch

   `git branch <branch-name>`

* List all available branches

   `git branch`

* Merge a branch from the current branch

    `git merge <branch-to-be-merged>`

* Check status of files

   `git status`

* Remove files for commit

   `git rm <file-name>`

* Pull - Update local repo with latest update from server

    * To pull from a single remote

        `git pull`

    * To pull from all remotes

        `git pull --all`

* Stash - Save changes made in the current index and working directory for later

    `git stash`

* Stash Apply - Apply stashed changes

    `git stash apply`

* See most recent stash without applying it

   `git stash show -p`

* View the content of an arbitrary stash

   `git stash show -p stash@{1}`

* Get Stash List

    `git stash list`

* Modify the Previous Commit's Message

    `git commit --amend -m "New commit message"`

* View commits of a certain author

    `git log --author=<username>`

* View all commits

    `git log`

* View list of tags

    `git tag`

* Config value for color
  
    ```
    color.status=auto
    color.interactive=auto
    color.diff=auto
    ```

* Export Git repository as a ZIP file

    `git archive --format=zip -9 HEAD -o <file-name>`

* Search (say, "foobar")

    `git grep "foobar"`

* Revert to previous version of a particular file

    1. Get the commit history of the file

        `git log path/to/file`

    2. Checkout to particular version using the commit hash obtained from the above command

        `git checkout <hash> path/to/file`

## Author

Bapusaheb Patil

<img src="https://github.com/bapspatil.png" width="20%">

https://bapspatil.com

## License

    This repository and its contents are licensed to Bapusaheb Patil, under the Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0) license.