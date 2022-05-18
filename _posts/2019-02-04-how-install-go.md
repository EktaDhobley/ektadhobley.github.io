---
layout: post
title:  "How to install Go on Apple M1 MacBook?"
summary: "Getting Started with Go"
author: Ekta Dhobley
date: '2022-04-13 14:35:23 +0530'
category: go
thumbnail: /assets/img/posts/golang.png
keywords: devlopr jekyll, how to use devlopr, devlopr, how to use devlopr-jekyll, devlopr-jekyll tutorial,best jekyll themes
permalink: /blog/welcome-to-devlopr-jekyll/
usemathjax: true
---


How to install Go on Apple M1 MacBook?
First, go to https://go.dev/, from there you click on 'Download'

Next, you will select the 'Apple macOs' option or the 'go1.18.1.darwin-arm64.tar.gz'

Once that is installed, you will just follow the installation process, by clicking 'Continue' and complete the next steps: (you can check where your Go is installed by using the shortcut 'Ctrl + Shift + J' in order to check your downloads and then opening it in 'Finder').

After that is done, open 'Terminal', you can check where your Go is installed by writing 'which go' in the terminal.

Follow the next steps to change the directory :

Now, we will set the path using the following command :
export GOROOT=/usr/local/go
Now we need to add the Go path over here. Go path will be where you will create your projects, your working directory.
On any choice of your folder, you can create the 'go-workspace' directory:
Now use the following command :
cd ~/
ls

Here you will see the 'Documents' folder.

Write the following commands in order to change the directory, here you will find your 'go-workspace' folder.

We will export the Go path over here using the following command:
Now we need to add the Go path and Go root to our path variable using the following command :
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

We can check the go version now, and we can see it's successfully installed using the following command :
go version

Install the dependency management tool for Go using the following command :
go install github.com/kardianos/govendor@latest

If you now go to the 'go-workspace' folder and then 'bin', inside that you will find the 'govendor' installed.
Done! You are set to use Go now.

