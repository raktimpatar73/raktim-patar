+++
date = "2019-06-10"
title = "How I created this site"
slug = "how-i-created-this-site"
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
<br>

### Step 1. Setting Up Hugo

For this read my previous blog on [Getting started with Hugo in Ubuntu](/posts/hugo-for-ubuntu/)

### Step 2. Starting a new project

Start a new project by using the below commands.
```
$ cd Desktop
$ hugo new site mysite
```
You can give any name to your site, just write your desired project name instead of 'mysite'

```
$ cd mysite
$ hugo server
```

Change to your project directory and start hugo server to view your first ever hugo project. You can then view your site on ['http://localhost:1313'](http://localhost:1313)

OMG! This is a blank page. If you are getting a blank page, Don't Worry! It's just the initial page where you can start creating your own site from scratch but let's not go through all that and choose a theme for your first project. 

### Step 3. Choosing a theme for your first project

Now let's cons further steps we would require a theme that you can select from hugo's themes [page](https://themes.gohugo.io/)

Explore a little and choose the theme of your choice, for this tutorial we would consider [this](https://themes.gohugo.io/hugo-coder-portfolio/) theme.

### Step 4. Downloading the theme

The theme can e downloaded either from the site directly or you can follow the below steps:

```
$ git clone https://github.com/naro143/hugo-coder-portfolio themes/coder-portfolio
```
This is how most of the users proceed with their projects. But it's generally advised to follow the steps below

```
$ git init
$ cd themes
$ git submodule add https://github.com/naro143/hugo-coder-portfolio 
```
Hurray you have installed your first theme successfully. Now just copy the **config.toml** from the example site folder inside this theme of yours and paste it on your projects root. Now again view you site in your web browser.

And Voila! Your first site using Hugo

### Step 5. Creating your first post

Now with everything setup, you can finally start writing your first post.
Create a markdown file and place it in your content folder or you can replace this folder wiht the content folder inside our example site.

```
$ cd content
$ touch my-first-post.md
```
Edit this file with your desired text editor and your first post is ready.
And Don't forget to play around with other themes and features. 

For further details [**Click Here**](https://gohugo.io/documentation/)
