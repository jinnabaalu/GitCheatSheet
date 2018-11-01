# Git Cheat Sheet

![Components of Cassandra](./images/git-logo.png)

## USE CASES

- [home](https://github.com/JinnaBalu/GitCheatSheet#clone-the-existing-repositoty)
- [git init](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-init.md#git-init)
- [git push with ssh](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-push-with-ssh.md#setup-git-push-with-ssh)
- [push local changes to repository]()

## Local Changes

##### Changed files in your working repo

```bash
git status
```

##### Chnages in tracked files

```bash
git status
```

##### Add all current changes 

```bash
git add --all
```

OR

```bash
git add .
```

##### commit all local changes in tracked files

```bash
git commit -am "my commit message"
```

**a-** all

**m-** message

## Commit History

##### Show all commits, starting with the newest

```bash
git log
```

##### Commit history of specific file

```bash
git log -p <file_name>

# EXAMPLE
git log -p README.md
```

##### Commit hitory by user

```bash
git blame <file_name>

#Example
git blame README.md
```

## Branches

##### List all local brnahces

```bash
git branch
```

##### List all local and remote brnahces

```bash
git branch -av
```

##### Switch to existing branch

```bash
git checkout <branch_name>

# Example
git checkout jinnabalu/testBranchName
```

##### Create a new branch

```bash
git checkout -b <brach_name>

# Example
git checkout -b jinnabalu/myNewBranchName
```

##### Delete local branch

```bash
git branch -d <branch_name>

# Example
git branch -d jinnabalu/myNewBranchName

## Force delete if not merged
git branch -D jinnabalu/myNewBranchName
```

##### Delete remote/origin branch

```bash
git push origin --delete <branch_name>

# Example
git push origin --delete jinnabalu/myNewBranchName
```

## Pull and Push


##### Get latest from remote

pull: gets latest pushed by someone to the branch

```bash
git pull
```

##### Push local changes

push: push local cahnges to the remote branch

```bash
git push -u origin <branch_name>

# Example
git push -u origin jinnabalu/myNewBranchName
```

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