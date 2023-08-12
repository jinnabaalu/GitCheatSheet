# Create the Git Remote Repository

When to go to the remote repository

- If there is more than one contributor
- If you don’t trust your machine disk, it may get crashed anytime
- Exchange the code change between the servers for writing the code in IDE in the dev machine, for deploy in the production server

With the [git init](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-init.md) local, we are done with creating the local repository, now we’ll create a remote repository in git host providers.

## Steps
1. Create the github account
2. Create the repository

### Create the Account
You have come here, hopefully you already have the account. These are very basic steps to create any "Generic Social Network Account Creation". 

### Create the Repository

- Goto Dashboard [github.com](https://github.com)
- Click on the New button on the left pan

![Create the git repository](./images/create-repo-new-button.jpg)

- Fill in the details required
![Fill Repository Details](./image/create-repository-details.jpg)
    - name of your choice
    - description about the repo 
    - public - if you want to opensource it.
    - private if you have a application logic which you can't opensource. 
    - Ignore other options
- Now you are in the instructions page, where you can get the 3 options to push your code to the created repo
![Instruction to push local repo to remote repo](./image/push-to-remote-repo.jpg)
- Go back to the  [git init](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-init.md) and use the option commands from the above picture.
    -  create a new repository on the command line
    ```bash
    echo "# test-repo" >> README.md
    git add .
    git commit -m "first commit"
    git branch -M main
    # Change your repo url
    git remote add origin git@github.com:JinnaBalu/test-repo.git
    git push -u origin main
    ```

> Note: While executing the above command you need to be aware of the `https` or `git` URL for pushing the changes. Initially use the `https` url only. If you still face issues [git-push-with-ssh](https://github.com/JinnaBalu/GitCheatSheet/blob/master/use-cases/git-push-with-ssh.md) 