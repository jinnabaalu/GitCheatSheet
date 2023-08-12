# Git Init

- Create the directory 
- Change to directory
- Initialize the directory with git and check for hidden folders in the directory


`git init`, to initiate the current directory to connect to the version controlling system or any git server

```bash
mkdir learn-git/
cd learn-git/
git init
```

> O/P : Initialized empty Git repository in `learn-git` directory

- After initializing the repository, it will create the hidden folder in the directory `/home/user/current-path/learn-git`.
- To view hidden fine in direct `Ctrl + H`
- Directory file structure looks like this

```bash
---
root
    branch/
    config
    description
    HEAD
    hooks/
        applypatch-msg.sample
        commit-msg.sample
        fsmonitor-watchman.sample
        post-update.sample
        pre-applypatch.sample
        pre-commit.sample
        prepare-commit-msg.sample
        pre-push.sample
        pre-rebase.sample
        pre-receive.sample
        update.sample
    info/
        exclude
    objects/
        info/
        pack/
    refs/
        heads/
        tags/
```
