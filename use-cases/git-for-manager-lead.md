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