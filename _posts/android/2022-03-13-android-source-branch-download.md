---
layout: post
title: "Steps to download certain branch Android source"
date: 2022-03-13 20:05:01
category: android
tags: [Android, source, repo]
---
install ubuntu on win11, then logon to ubuntu.

install git 
```
sudo apt-get install git
whereis python
sudo ln -s /usr/bin/python3.8 /usr/bin/python
```

```
mkdir ~/bin
PATH=~/bin:$PATH
```

```
curl https://mirrors.tuna.tsinghua.edu.cn/git/git-repo  > ~/bin/repo
chmod +x ~/bin/repo
```

```
vim ~/.bashrc
export REPO_URL='https://mirrors.tuna.tsinghua.edu.cn/git/git-repo'
source ~/.bashrc
```

```
mkdir WORKING_DIRECTORY
cd WORKING_DIRECTORY
```

```
repo init -u https://mirrors.tuna.tsinghua.edu.cn/git/AOSP/platform/manifest -b android-5.1.0_r1
repo sync
```

branches view: https://source.android.com/setup/start/build-numbers#source-code-tags-and-builds
