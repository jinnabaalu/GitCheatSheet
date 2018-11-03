# Switching remote URLs from HTTPS to SSH

## List existing URLs

- List your existing remotes in order to get the name of the remote you want to change.


```code
git remote -v
```

> O/P

> origin	git@github.com:JinnaBalu/jinnabalu.github.io.git (fetch)
> origin	git@github.com:JinnaBalu/jinnabalu.github.io.git (push)

## Change your remote's URL

- Change your remote's URL from SSH to HTTPS with the `git remote set-url` command.

```bash
git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```
