# Branch Management

Consider *master* branch as the single branch for both prod and dev

## Steps to create a branch and merge the branch to master

### **Step 1** checkout to master and create a branch

```bash
git checkout master

git checkout -b JinnaBalu/Sample
```

JinnaBalu/Sample - branch name, choose as you like

> NOTE: Good practice to follow some Naming Convention to create branch names but not mandatory
> JinnaBalu is the github user name and JinnaBalu/Sample is the branch name**

### **Step 2** -  As you are done with some changes to the code, follow

```bash
git status

git add --all

git commit -am "message related to changes done in the branch"

git status

git push -u origin JinnaBalu/Sample
```

**-a** = all, **m** = message, push all your changes to your remote or origin branch

### Step 3 - Merge the newly created branch to master

**Step 3.1** - Get the latest from the master, considering that contributors are more than one member

```bash
git checkout master

git pull
```

**Step 3.2** - Merge master to your branch

```bash
git checkout JinnaBalu/Sample

git merge --no-ff origin master
```

You may get conflicts here if someone modified the same file which you modified

Need to resolve conflicts if any and repeat **Step 2**

**Step 3.3** - Merge your branch to master

```bash
git checkout master

git merge --no-ff origin JinnaBalu/Sample
```

This completes the flow of basic branching
