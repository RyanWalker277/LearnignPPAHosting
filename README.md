# LearnignPPAHosting
This repo is meant for learning to host a PPA repo over github. This will contain a sample hello world deb package and it will be made avaialbe for install through apt over linux systems

# Description

This ppa holds a basic hello world package.

# Install Instrctions

```console
curl -s --compressed "https://innogeeks.me/LearningPPAHosting/PPA/hello.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/hello.gpg >/dev/null
```

```console
curl -s --compressed -o /etc/apt/sources.list.d/packageList.list "https://innogeeks.me/LearningPPAHosting/PPA/packageList.list"
```

```console
apt update
```

```console
apt install hello
```
Run the package by a simple `hello` command