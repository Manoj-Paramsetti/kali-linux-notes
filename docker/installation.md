# Docker
### Requirements:<br>
**Architecture**<br>
Docker Engine is supported on x86_64 (or amd64), armhf, and arm64<br>
**Debain** <br>
Debian Bullseye 11 (testing)<br>
Debian Buster 10 (stable)<br>
Raspbian Bullseye 11 (testing)<br>
Raspbian Buster 10 (stable)<br>

## Installation
```bash
$ sudo apt update
$ sudo apt install -y docker.io
$ sudo systemctl enable docker --now
$ docker
```
Changing group for docker to use in your account
```bash
$ sudo groupadd docker
$ sudo usermod -aG docker $USER
```
Open nautilus in root
```bash
$ su
$ nautilus
```
Now go to `/etc` select `docker/` folder then change properites for non-root user as create and delete files

**Now logout and login again**

Add mirror
```bash
$ printf "%s\n" "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-ce-archive-keyring.gpg] https://download.docker.com/linux/debian buster stable" \
  | sudo tee /etc/apt/sources.list.d/docker-ce.list
```

Import key
```bash
curl -fsSL https://download.docker.com/linux/debian/gpg \
  | gpg --dearmor \
  | sudo tee /usr/share/keyrings/docker-ce-archive-keyring.gpg
```

Now, Install docker-ce, docker-ce-cli, containerd.io
```
$ sudo apt update
$ sudo apt install docker-ce docker-ce-cli containerd.io -y
```

Starting docker and containerd service at boot
 ```sudo
 sudo systemctl enable docker.service
 sudo systemctl enable containerd.service
 ```
 
**Now, Restart your machine**

## 
