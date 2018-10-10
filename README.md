
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

7. Changing a remote URL for your repository  

    `git remote set-url origin <repository-url>.git`

8. Push - Update changes to repository on GitHub

    8.1 To push to `master` branch
  
        git push -u origin master

    8.2 To force-push (**Warning**: This erases all previous commits)

        git push -u origin master -f

    8.3 To push to a different branch
  
        git push -u origin <branch-name>

9. Clone a repository

   `git clone <repository-url>`

10. Create a new branch from current working branch and switch to it

    `git checkout -b <new-branch-name>`

11. Create new branch from an existing branch and stay in the current branch

    `git checkout -b <new-branch> <existing-branch>`  

12. Switch to a new branch

    `git branch <branch-name>`

13. List all available branches

    `git branch`  

14. Delete a branch

    `git branch -d <branch-name>`

15. Merge a branch from the current branch

    `git merge <branch-to-be-merged>`

16. Check status of files

    `git status`

17. Remove files for commit

    `git rm <file-name>`

18. Pull - Update local repo with latest update from server

    18.1 To pull from a single remote

        git pull

    18.2 To pull from all remotes

        git pull --all

19. Stash - Save changes made in the current index and working directory for later

    `git stash`

20. Stash Apply - Apply stashed changes

    `git stash apply`

21. See most recent stash without applying it

    `git stash show -p`

22. View the content of an arbitrary stash

    `git stash show -p stash@{1}`

23. Get Stash List

    `git stash list`

24. Modify the Previous Commit's Message

    `git commit --amend -m "New commit message"`

25. View commits of a certain author

    `git log --author=<username>`

26. View all commits

    `git log`

27. View list of tags

    `git tag`

28. Config value for color
  
    ```
    color.status=auto
    color.interactive=auto
    color.diff=auto
    ```

29. Export Git repository as a ZIP file

    `git archive --format=zip -9 HEAD -o <file-name>`

30. Search (say, "foobar")

    `git grep "foobar"`

31. Revert to previous version of a particular file

    31.1 Get the commit history of the file

        git log path/to/file

    31.2 Checkout to particular version using the commit hash obtained from the above command

        git checkout <hash> path/to/file

32. Reapply commits on top of another base tip

    `git rebase <branch-name>`

## Author

Bapusaheb Patil

<img src="https://github.com/bapspatil.png" width="20%">

https://bapspatil.com

## License

    This repository and its contents are licensed to Bapusaheb Patil, under the Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0) license.