

### 1. Creating a Branch
To create a new branch, you use:
```sh
git branch <branch-name>
```
This creates a new branch named `<branch-name>` but does not switch to it.

### 2. Listing Branches
To list all branches in the repository, you use:
```sh
git branch
```
The command will show all branches, with an asterisk (*) next to the currently active branch.

### 3. Switching to a Branch
To switch to a different branch, you use:
```sh
git checkout <branch-name>
```
Alternatively, in newer versions of Git (2.23 and later), you can use:
```sh
git switch <branch-name>
```
This command checks out the specified branch, making it the current working branch.

### 4. Creating and Switching to a Branch
You can combine the creation and switching of branches with:
```sh
git checkout -b <branch-name>
```
Or using the newer syntax:
```sh
git switch -c <branch-name>
```
This command creates a new branch and switches to it immediately.

### 5. Renaming a Branch
To rename the current branch, you use:
```sh
git branch -m <new-branch-name>
```
If you need to rename a branch that you are not currently on, use:
```sh
git branch -m <old-branch-name> <new-branch-name>
```

### 6. Deleting a Branch
To delete a local branch that is not currently checked out, use:
```sh
git branch -d <branch-name>
```
If the branch has unmerged changes and you want to forcefully delete it, use:
```sh
git branch -D <branch-name>
```

### 7. Merging a Branch
To merge changes from one branch into the current branch, you use:
```sh
git merge <branch-name>
```
This command merges the specified branch into the current branch.

### 8. Viewing Branch History
To see a graph of the branch history, you can use:
```sh
git log --graph --oneline --all --decorate
```
This command provides a visual representation of the branching history.

### 9. Tracking Remote Branches
To see remote branches, use:
```sh
git branch -r
```
To create a local branch that tracks a remote branch, use:
```sh
git checkout -b <local-branch-name> origin/<remote-branch-name>
```

### 10. Pushing Branches
To push a branch to a remote repository, use:
```sh
git push origin <branch-name>
```
If you want to push all branches to the remote repository, use:
```sh
git push --all
```

### 11. Pulling from Remote Branches
To pull changes from a remote branch to your local branch, use:
```sh
git pull origin <branch-name>
```
This command fetches and integrates changes from the specified remote branch into your current branch.

