# Proof of Work

## Git Log Output

```
564762f (HEAD -> main, origin/main) initial commit with deploy script
```

## Reflection Questions

## Reflection Questions

### Q1: What is the difference between Git and GitHub?

Git is a local version control system that tracks changes to files on your own computer. It works completely offline and handles commits, branches, and merges. GitHub is a cloud-based platform that hosts Git repositories online. It adds collaboration features such as Pull Requests, issue tracking, and access control. In short, Git is the tool, while GitHub is a service built around that tool.

### Q2: Explain the three architecture stages: Working Directory, Staging Area, and Local Repository.

The Working Directory is where you create and edit your files directly. The Staging Area (also called the index) holds the changes you have marked with `git add`, which are ready to go into the next commit. The Local Repository, stored in the hidden `.git` folder, permanently saves the committed snapshots of your project. The typical flow is: Working Directory, then `git add` to the Staging Area, then `git commit` to the Local Repository.

### Q3: What is the difference between git stash pop and git stash apply?

Both commands restore stashed changes back into your working directory. `git stash pop` applies the changes and then removes that entry from the stash list. `git stash apply` applies the changes but keeps the entry in the stash list. This makes `apply` useful when you want to reuse the same changes on multiple branches, while `pop` is better when you no longer need the stash afterwards.

### Q4: What is the difference between git fetch and git pull?

`git fetch` downloads new commits and branches from the remote repository but does not change your current working branch. It lets you review what has changed before deciding to integrate it. `git pull` is essentially `git fetch` followed by `git merge`, so it updates your current branch immediately. Because of this, `fetch` is safer and more controlled, while `pull` is faster and more convenient.
