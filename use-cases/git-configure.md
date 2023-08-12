# Configure git

## Description

`git config` helps you set your email and name for your commit, we can't change the committer names after the commit. Every contributor will have their identification on every commit.
    
We can configure git at two levels, at the repository level, and global.
    
## Global Config

```
git config --global user.name "Your Name"
git config --global user.email yourmail@domain.tld
```

Repository Config - useful when you work with multiple business emails:
```
git config --global user.name "Your Name"
git config --global user.email yourmail@domain.com
```
