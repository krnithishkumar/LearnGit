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
