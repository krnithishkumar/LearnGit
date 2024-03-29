## Git Commands
1. Initialize - `git init`
2. Create New Branch - `git checkout -b <branch-name>`
## Git stash
3. This command temporarily stores all the modified tracked files. - `git stash save`
4. This command restores the most recently stashed files. - `git stash pop`
5. This command lists all stashed changesets. - `git stash list`
6. This command discards the most recently stashed changeset. - `git stash drop`
## Git Merge
### Fast Forward Merge
7. Start a new feature - `git checkout -b new-feature main`
8. Edit some files
`git add <file>`
`git commit -m "Start a feature"`
9. Merge in the new-feature branch
`git checkout main`
`git merge new-feature`
`git branch -d new-feature`
### 3-way merge
9. Start a new feature
`git checkout -b new-feature main`
10. Edit some files
`git add <file>`
`git commit -m "Start a feature"`
11. Edit some files
`git add <file>`
`git commit -m "Finish a feature"`
12. Develop the main branch
`git checkout main`
13. Edit some files
`git add <file>`
`git commit -m "Make some super-stable changes to main"`
14. Merge in the new-feature branch
`git merge new-feature`
`git branch -d new-feature`
## Git push
15. Push command is used to upload local repository content to a remote repository. 
`git push <option> [<Remote URL><branch name><refspec>...]`
## Git pull
16. Pull command is used to get the updates from remote repository to a local repository content.
`git pull <option> [<repository URL><refspec>...]`
## Git diff
17. To show the difference between current working directory and last commit
`git diff HEAD`
## Undoing things
18. To modify a most recent commit. It lets you combine staged changes with the previous commit instead of creating an entirely new commit.
`git commit --amend`
## How to setup your Git user email
19. To setup the user email address you'll use in your commits.
`git config --global user.email "<your_email_id>"`
# How to cache your login credentials in Git
20. To store login credentials in the cache, so you don't have to type them in each time.
`git config --global credential.helper cache`