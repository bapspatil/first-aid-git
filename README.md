
# first-aid-git

A quick guide and list of commands related to Git & GitHub.
<br>If you're new to Git and GitHub or want to deepen your knowledge about it, this repository is for you.

**Feel free to email any doubts you may have at <a href="mailto://hi@bapspatil.com">hi@bapspatil.com</a>.**

## Here you go:

1. Configuring the username in Git

    `git config --global user.name "Firstname Lastname"`

    * To display the username set

        `git config --global user.name`

2. Configuring email in Git

    `git config --global user.email "youremail@example.com"`

    * To display the email set

        `git config --global user.email`

3. Create a new local Git repository

    `git init`

4. Add files for commit

    4.1 To add all files in the current folder/directory

        git add .

    4.2 To add a single file

        git add <file-name>

    4.3 To add multiple files

        git add <file-1> <file-2>

5. Commiting files

   `git commit -m "Descriptive commit message"`

6. Adding a remote, i.e. the GitHub URL for your repository

    `git remote add origin <repository-url>.git`

7. Push - Update changes to repository on GitHub

    7.1 To push to `master` branch
  
        git push -u origin master

    7.2 To force-push (**Warning**: This erases all previous commits)

        git push -u origin master -f

    7.3 To push to a different branch
  
        git push -u origin <branch-name>

8. Clone a repository

   `git clone <repository-url>`

9. Create a new branch from current working branch and switch to it

   `git checkout -b <new-branch-name>`

10. Create new branch from an existing branch and stay in the current branch

    `git checkout -b <new-branch> <existing-branch>`

11. Switch to a new branch

    `git branch <branch-name>`

12. List all available branches

    `git branch`

13. Merge a branch from the current branch

    `git merge <branch-to-be-merged>`

14. Check status of files

    `git status`

15. Remove files for commit

    `git rm <file-name>`

16. Pull - Update local repo with latest update from server

    16.1 To pull from a single remote

        git pull

    16.2 To pull from all remotes

        git pull --all

17. Stash - Save changes made in the current index and working directory for later

    `git stash`

18. Stash Apply - Apply stashed changes

    `git stash apply`

19. See most recent stash without applying it

    `git stash show -p`

20. View the content of an arbitrary stash

    `git stash show -p stash@{1}`

21. Get Stash List

    `git stash list`

22. Modify the Previous Commit's Message

    `git commit --amend -m "New commit message"`

23. View commits of a certain author

    `git log --author=<username>`

24. View all commits

    `git log`

25. View list of tags

    `git tag`

26. Config value for color
  
    ```
    color.status=auto
    color.interactive=auto
    color.diff=auto
    ```

27. Export Git repository as a ZIP file

    `git archive --format=zip -9 HEAD -o <file-name>`

28. Search (say, "foobar")

    `git grep "foobar"`

29. Revert to previous version of a particular file

    29.1 Get the commit history of the file

        git log path/to/file

    29.2 Checkout to particular version using the commit hash obtained from the above command

        git checkout <hash> path/to/file

30. Reapply commits on top of another base tip

    `git rebase <branch-name>`

## Author

Bapusaheb Patil

<img src="https://github.com/bapspatil.png" width="20%">

https://bapspatil.com

## License

    This repository and its contents are licensed to Bapusaheb Patil, under the Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0) license.