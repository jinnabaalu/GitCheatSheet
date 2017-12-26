# Git Cheat Sheet

## Clone the existing repositoty

```bash
git clone <CLONE_URL>

# Example
git clone https://github.com/JinnaBalu/GitCheatSheet.git
```

## Init the local git

```bash
git init
```

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

**a-all**
**m-message**

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


