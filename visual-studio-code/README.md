## Installing VS Code

***Notice: Don't include the $ (dollar) sign in the commands***

First, we want to check and install some dependencies
```bash
$ sudo apt-get update
$ sudo apt-get install curl gpg software-properties-common apt-transport-https 
```
Then add the key
```bash
$ curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
```
Then link VSCode repo with apt
```bash
$ echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" | sudo tee /etc/apt/sources.list.d/vscode.list
```

Now, you are all done for now, just run these two commands then use VSCode
```bash
$ sudo apt-get update
$ sudo apt-get install code -y
```
---
## To update
```bash
$ sudo apt-get update
$ sudo apt-get upgrade -y
```


**Happy Hacking!!** 
