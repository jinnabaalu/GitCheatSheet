# Common Commands using git

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

##### Commit history by user

```bash
git blame <file_name>

#Example
git blame README.md
```

## Branches

##### List all local branches

```bash
git branch
```

##### List all local and remote branches

```bash
git branch -av
```

##### Switch to an existing branch

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

##### Delete the local branch

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


##### Get the latest from remote

pull: gets latest pushed by someone to the branch

```bash
git pull
```

##### Push local changes

push: push local changes to the remote branch

```bash
git push -u origin <branch_name>

# Example
git push -u origin jinnabalu/myNewBranchName
```
