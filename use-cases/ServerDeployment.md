# Deploy and update git repository on a hosted server

These steps assume that the origin of the repository is on a web-based hosting service such as GitHub or BitBucket.

#### **Step 1** Clone a copy of the repository to the server

```bash
ssh yourusername@yourdomain.com
```

Enter you password, and then navigate to the required folder location.

```bash
cd /path/to/folder
```

Clone the repository

```bash
git clone http://bitbucket.com/your-repository
```

**Now that the repository is on the server, lets see how we would update it after making local changes**

#### **Step 2** Update with local repo changes

Let's add a new file to the local repo, commit the changes, and push to origin

```bash
cd ~/my-local/repo
touch new-file.txt
git add .
git commit -m "added new-file.txt"
git push orgin master
```

The new file is now on the BitBucket repo, but not on our web hosting sever. So, we need to ssh back into it, and pull the changes from origin.

```bash
ssh yourusername@yourdomain.com
cd /path/to/repo
```

Now if we run 'git status' you will see that the repo is up to date. This is because we need to ge the latest commit details from origin

```bash
git remote update
```

And pull the changes

```bash
git pull
```






