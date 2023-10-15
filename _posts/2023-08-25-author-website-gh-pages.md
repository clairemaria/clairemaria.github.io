---
layout: post
read_time: true
show_date: true
title:  Author Websites with Github Pages
date:   2023-08-24 15:14:20 -0600
description: "Custom author websites can rock branding... but how to you set one up for free?"
img: posts/20230824/computerScreen.jpeg
tags: [websites, github, DIY]
author: Vera Briene
toc: no  # leave empty or erase for no TOC
---

## Why?

Do you like this website? It was free! In this guide, I'll drag you a high-level process for building THIS VERY WEBSITE (wow!) with GitHub Pages. If you don't have prior coding knowledge, this article might not be enough.

GitHub has great articles on how to complete this process, but I want to document the gotchas I experienced while setting up this bomb-ass site. 

> P.S. GitHub can do other cool things for authors too. [Here's one author's experience with git](https://www.gitkraken.com/gitkon/git-for-writers).

### Nice-To-Haves

- Prior coding knowledge or the time to learn
- Command line knowledge

## 1. Github

Match your author name to your [GitHub](www.github.com) account username. I (Vera Briene) might pick `verabriene` as my GitHub account name.

If you're new to git, consider using a tool like [Git Kraken](https://www.gitkraken.com/) to organize your project. 

### Make the Project

Pick where your code will live. Each website will live in it's own project (works like a computer folder). To create a new project, follow [this guide](https://docs.github.com/en/pages/quickstart#creating-your-website).

Complete "Creating Your Website", skip the last section "Change Title and Description." We'll deal with the title later.

SO IMPORTANT!! This sets your default website URL, so use your author name! For me, that might be -
- `verabriene.github.io`
- `authorverabriene.github.io`
- `vbriene.github.io`

GitHub will give you these domain names for free, as long as they end in `github.io`. 

Your live website will live at `www.yourname.github.io`. It won't work quite yet, though.

This is where I might have lied to you. To get the *optional* cute URL `www.yourname.com`, have to pay a yearly domain fee (usually $12) for the name. I buy mine from Google Domains. [Setting up custom domain names can be found here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

### Install Tools

Install the following tools to create your website -
- **Jekyll** builds your website! [Here are the instructions.](https://jekyllrb.com/docs/installation/)
- **Visual Studio Code**. You may use Scrivener, Word, or Google Docs to write your novels. Visual Studio Code (VS Code) is a similar tool for developers. If it looks scary, remember it's just a fancy Microsoft Word. Download and install that [Here is the download.](https://code.visualstudio.com/download).

### Bring the Project to Your Computer

Let's bring the project to your computer. 

The workflow will be -
- Write content on your computer and test it
- Send it to GitHub
- Launch the website

> If this is brand new, find a coder friend and have them work alongside you. 

#### Git Clone

Use your terminal to `git clone` your repository. This brings the code to your computer to work on (like downloading an email attachment to open on your computer). [Here](https://youtu.be/8JJ101D3knE?si=kK52Btu97jP030ZT) is a great video on using git. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/8JJ101D3knE?si=gaChcmFbR_ee-c9u" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Changes in VS Code

Open the entire folder in VS Code. Consider downloading a Jekyll project plugin! You will be making changes in the `posts/` folder (we'll learn how later).

#### Jekyll Serve

Before making changes, test your installation with Jekyll. I chose to add the starter site first. Inside of your project folder, follow the instructions [here](https://jekyllrb.com/docs/).

Some tips -
- Reload the webpage (`localhost:4000`) after you make changes
- If your changes aren't showing, restart the `jekyll serve` command 

#### Git Commit + Push

Use git commands to `git add`, `git commit` and `git push`. *Your website won't launch until you do this*. Go to the URL you chose above, such as www.yourprojectname.github.io, and double-check that your website is present. 

#### Optional: Pick Branch Strategy

Some authors want to make a "work in progress" branch where they can save undeployed changes. This allows authors to commit and push changes without them going live on the website. 

I live by the YOLO principle and make changes directly on `main` because I am fastidious about checking my changes on my computer first. 

## Creating Content 

Now you want to add things to your website. By default, you can add markdown pages in the `_posts` folder, git commit them, and have your website. Figure out how to add a post now. Some tips -
- Copy and paste an existing post page. There should be one called "_posts/2023-08-26-welcome-to-jekyll.markdown".
- The post above tells you exactly what needs to go in a post.
- Play around with markdown files. [You can add links, images, and formatting](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

The banner pictures live in `assets/img/posts` in a folder with the date. Make sure your resolution is high enough (over 1500 pixels).

After this, the themeing is purely aesthetic. 

### Picking Themes

[I used this one](https://www.bestjekyllthemes.com/theme/the-mvm-the-mvm.github.io/). There are excellent instructions in his README to install.

**I wanted to make HTML and CSS changes**, so I went the route of downloading the project manually and copy-pasting into my project folder. To do this -
- Erase everything that already exists in the folder except your `.git` files.
- Paste. Make sure to exclude their `.git` files.

> Tip! Some folders (like `_site/`) are built every time you restart the server. Make sure to make changes in the top-level `assets/`, `_layout`, and `_include` folders if you're getting wild with code changes.

## Deployment and Beyond

Making changes to `_config.yml` is the last step to build your Jekyll project. For the theme above, I had to -
- Change the site settings at the top of the file
- Adjust the author settings
- Adjust the social media settings. These get tagged in every author element (an example is the author page and post pages toward the bottom)

If you need help, we can set up a one-on-one consult session, or you can check the newsletter for upcoming group classes. 

Enjoy!
