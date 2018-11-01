# Setup git push with ssh

## [Github](https://github.com/)

### Create the rsa key in local machine

```bash
ssh-keygen -t rsa -C "your_github_email@example.com"
```

> Note : In local machines we may have multiple ssh keys, better to create the specific rsa. 
> Example : Enter file in which to save the key `(/home/ubuntu/.ssh/id_rsa): /home/ubuntu/.ssh/github_rsa`

```bash
O/P:

Generating public/private rsa key pair.
Enter file in which to save the key (/home/ubuntu/.ssh/id_rsa): /home/ubuntu/.ssh/github_rsa
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/ubuntu/.ssh/github_rsa.
Your public key has been saved in /home/ubuntu/.ssh/github_rsa.pub.
The key fingerprint is:
SHA256:vddr6bSmZdqSM0/6pIo5g+yiycMZRMetgp70NuCcRcM *******@outlook.com
The key's randomart image is:
+---[RSA 2048]----+
|  .. .           |
|  .Eo .          |
| o....           |
|.oo..    .       |
|=.*.    S .      |
| *.+       . .   |
| ..o.. .  . ..B. |
| .+.. o oo .=@+o |
|  +o o. oo..=@B  |
+----[SHA256]-----+
```