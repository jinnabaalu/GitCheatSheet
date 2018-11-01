# Git Cheat Sheet

![Components of Cassandra](./images/git-logo.png)

## USE CASES

- [home](https://github.com/JinnaBalu/GitCheatSheet#clone-the-existing-repositoty)
- [git init](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-init.md#git-init)
- [git push with ssh](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-push-with-ssh.md#setup-git-push-with-ssh)
- [push local changes to repository](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-commit-file.md#committing-files)
- [create new branch](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/create-branch.md#create-branch)
[- branch management]()
- [common git commands](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/commonly-used-commands.md#common-commands-using-git)
- [delete commits](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/delete-commits.md#remove-the-last-commitcommits-using-reset)

## GIT MERGE

Merging changes from feature_branch to develop

1. Get latest from develop and merge to feature_branch

```bash
git checkout develop

git pull

git checkout feature_branch 

git merge --no-ff origin develop
```

**Note : To be safe from conflict with develop(GOOD PRACTICE), we will resolve in feature_branch**

2. Merge feature_branch to develop

```bash
git checkout develop 

git merge --no-ff origin feature_branch 
```

## GIT RESET

1. Soft Reset

```bash
git reset <commit_hash> --soft
```

2. Mixed Reset

```bash
git reset <commit_hash>

#OR

git reset <commit_hash> --mixed
```

3. Hard Reset
```bash
git reset <commit_hash> --hard
```

# Git for Project Lead/Manager

1. Get count of branches

```bash
git branch -a | wc -l
```

2. Get the commits from individual

```bash
git shortlog -s -n --all

#OR

git shortlog -s -n
```

3. Get count the commits for the branch we are in

```bash
git rev-list --count HEAD

#OR

git log --pretty=oneline | wc -l

#OR

git rev-list --count <BRANCH_NAME>
```

4. List of branches

```bash
git branch -a
```