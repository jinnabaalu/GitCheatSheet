
# Update the remote URL 

#### Update the Remote URL of the repository with the ssh url in place of https

- Copy the url from the ![clone repository](../images/clone_repo.png) button with ssh

- Copy Clone with ssh URL - Clock *Use SSH* as in first screenshot

![click_use_ssh](../images/click_use_ssh.png) ![copy_ssh_url](../images/copy_ssh_url.png)

```bash
 git remote set-url origin git@github.com:JinnaBalu/GitCheatSheet.git
```

### 7. Test pushing with ssh

```bash
git add --all

git commit -am "testing the changes"

git push -u origin master
```

*DONE with Github*
