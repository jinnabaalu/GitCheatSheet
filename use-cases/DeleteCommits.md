# Remove the last commit/commits using Reset

## Steps to remove the last commit/commits

#### **Step 1** Checkout to master

```bash
git checkout master
```

This could be done in any branch. For this example, *master* branch is used.

#### **Step 2** -  Get the commits history

```bash
git log
```
You will end up with list of commits that you made as follows.

![logs](https://user-images.githubusercontent.com/22785263/47548190-d2dc6580-d915-11e8-8591-c470511ddae0.PNG)

#### Step 3 - Reset 

**Step 3.1** - Copy the commit-hash that you want to reset

All the commits that top of the selected commit-hash (not including the enterd commit-hash), will be deleted.

**Step 3.2** - Hard reset to go back to early stage

```bash
git reset <commit-hash> --hard
```

#### Step 3 - Force push to the repository

```bash
git push <remote> master --force
```

`<remote>` can be any remote, `origin` is the default.

Be careful when removing the previous commits, there is no going back once you did these changes.

