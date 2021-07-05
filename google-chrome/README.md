## Installation for google chrome

First, Download chrome deb package using wget
```bash
$ wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```
Don't change the directory and run this command
```
$ sudo apt-get install .$(pwd)/google-chrome-stable_current_amd64.deb
```
---
### Updating chrome

First, check you have source list for apt 
```
$ cat /etc/apt/sources.list.d/google-chrome.list
```

If it doesn't return anything, just run this command
```bash
$ echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" > /etc/apt/sources.list.d/google-chrome.list
```

Just run

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
```

**Happy Surfing!! :D**
