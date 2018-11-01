# GIT MERGE

Merging changes from feature_branch to develop

1. Get latest from develop and merge to feature_branch

```bash
git checkout develop

git pull

git checkout feature_branch

git merge --no-ff origin develop
```

> Note : To be safe from conflict with develop(GOOD PRACTICE), we will resolve in feature_branch

2. Merge feature_branch to develop

```bash
git checkout develop

git merge --no-ff origin feature_branch
```