+++ 
date = "2019-06-10"
title = "getting started with hugo in Ubuntu"
slug = "hugo-for-ubuntu" 
tags = [
    "go",
    "golang",
    "hugo",
    "development",
]
categories = [
    "Development",
    "golang",
]
+++
## Step 0. Installing Go

Hugo requires Go installed in your system. If you have Go already installed in your ubuntu version jump straight to the next section.
And for all other who are new to Go just follow along:

```
$ sudo apt-get update \
> sudo apt install snapd \
> sudo snap install --classic go
```
There are many other ways to install go, but this is the easiest one in my opinion for all those who does not want to go setting up an environment.

**NOTE :** This installation is meant for recent Ubuntu versions. Not tested for older versions.

## Step 1. Install Hugo

**Method 1:** Using apt
```
$ sudo apt-get install hugo
```
This method might lead to some issues due to apt being not able to install the latest version of hugo on your system.
Check with

```
$ hugo version
```
If the hugo version is not equal to the latest version follow the below steps.

<br>
**Method 2:** Downloading and Installing Hugo

Goto [hugo releases](https://github.com/spf13/hugo/releases) and download the latest extended .deb file for your os and architecture.<br>

Save it somewhere specific or install using Ubuntu's native Package manager that would work the same.

Or you can follow the manual way of extracting and installing it.

## Step 2. Using CLI
<br>

First we need to download the latest version of hugo
```
$ wget https://github.com/gohugoio/hugo/releases/download/{version}/{file name}
```

Then the below steps are for extracting, installing, removing the compressed file followed by checking of hugo version
```
$ sudo dpkg -i hugo_extended_0.55.6_Linux-64bit.deb
$ sudo rm hugo_extended_0.55.6_Linux-64bit.deb
$ sudo hugo version
```

This should give an output:

```
Hugo Static Site Generator v0.55.6-A5D4C82D2/extended linux/amd64 BuildDate: 2019-05-18T08:08:34Z
```

If you get such an output my friend we are ready to buld some beautiful static sites
If you want to knwo how I made this website don't forget to click on this link -> [How I created this site](/posts/how-i-created-this-site/)



