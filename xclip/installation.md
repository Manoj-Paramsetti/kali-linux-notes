# Installation steps for xclip


First get the updated version list for packages using apt
```bash
sudo apt-get update
```

Now, Install xclip using apt-get
```bash
sudo apt-get install xclip
```

Copy & Paste with xclip
----
Replace the `FILENAME_TO_COPY` with your filename with file extension
```bash
xclip -selection clipboard < FILENAME_TO_COPY
```

---

Add xclip shortcut (OPTIONAL)
----
For bash shell
```bash
echo "alias xclipboard='xclip -selection clipboard <'" >> ~/.bashrc
```

For zsh shell
```bash
echo "alias xclipboard='xclip -selection clipboard <'" >> ~/.zshrc
```

**Now, restart or open a new terminal to see the changes**
