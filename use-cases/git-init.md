# Git Init

`git init`, to initiate the current directory to connect to the version controlling system or any git server

```bash
git init
```

> O/P : Initialized empty Git repository in /home/user/current/directory-test

- After initializing the repository, it will create the hidden folder in the directory `/home/user/current/directory-test`.
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

## branch

- A deprecated way to store shorthands to be used to specify a URL to git fetch, git pull and git push. This mechanism is legacy and not likely to be found in modern repositories. Simplyfying it like no use of it in modern repositories.