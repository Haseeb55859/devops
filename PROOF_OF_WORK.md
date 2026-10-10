# Proof of Work

## Git Log
71ce1bc (HEAD -> main, origin/main) Merge pull request #1 from Haseeb55859/development
ebd3f57 (origin/development, development) Resolve merge conflict between development and staging
ed02d7f (origin/staging, staging) Update deploy.sh for staging environment
50f6157 Update deploy.sh for development environment
8cd1279 Initial commit: add deploy.sh and README.md

## Reflection Questions

**Q1: Git vs GitHub**
Git is a local version control system that tracks changes in files on your own computer. GitHub is a cloud platform that hosts Git repositories online. It allows teams to collaborate through features like pull requests and issues. Git works offline, while GitHub needs internet. In short, Git is the tool and GitHub is the service built around it.

**Q2: Three Architecture Stages**
The Working Directory is where you create and edit files. The Staging Area is an intermediate zone where you select which changes go into the next commit using `git add`. The Local Repository stores the committed snapshots permanently in the .git folder. Files move from Working Directory to Staging Area to Local Repository.

**Q3: git stash pop vs git stash apply**
Both restore stashed changes into the working directory. `git stash pop` applies the changes and then removes them from the stash list. `git stash apply` applies the changes but keeps them in the stash list. Apply is useful when you want to reuse the same stash on multiple branches.

**Q4: git fetch vs git pull**
`git fetch` downloads new commits from the remote but does not change your working files. `git pull` is fetch plus merge, so it downloads and immediately merges changes into your current branch. Fetch is safer because you can review changes first. Pull is faster but can cause merge conflicts.