---
title: My Personal Website (GitHub+Hexo)
date: 2019-11-20 16:31:39
tags: blog
cover_detail: /assets/pw5.png
---

This personal website is built mainly by using the blog framework [Hexo](https://hexo.io/ " ") and github. Here are some notes.

## Steps to build this website

-   Get a personal domain name
    The domain name "idandelion.com" is gotten from the name server Namesilo. I chose this name since I like the flower dandelion and it contains my name as well, and of course, it is easy to remember.   

-   Build a new repository in GitHub
    Build a repository with the name "username.github.io", for example, mine is danliudl.github.io.

-   Install Git/Node.js/Hexo
    I already have git and node.js in my computer, so I only need to install Hexo:
        npm install hexo-cli -g
        hexo init blog
        cd blog
    
-   Deploy website in GitHub
    This step is to deploy the hexo website in GitHub, first install the plugin hexo-deployer-git:
        npm install hexo-deployer-git --save
    then edit the file _config.yml:
        deploy:
        type: git
        repo: https://github.com/Danliudl/danliudl.github.io.git
        branch: master

-   Bind the personal domain name
    Now I can use the url https://danliudl.github.io to reach the website. However, I prefer to use my own domain name, so I edited the dns records in the name server and then changed the setting of GitHub to add the custom domain. Till now, I can use the personal domain name to reach the website.

-   Change the website theme
    Hexo provides customizable themes for users, here I used the theme [Phantom](https://github.com/klugjo/hexo-theme-phantom).

-   Customize the website
    -   Designed and added the logo to the website
    -   Modified the code to support post categories
    -   Added responsive videos

-   Useful tools
    -  [TinyPNG](https://tinypng.com/) : to compress PNG images while preserving transparency to get better loading performance of webpages
    -  FireShot: chrome plugin, to capture full web page screenshots
    -  Browsersync: time-saving synchronized browser testing


Reference:
https://hexo.io/docs/
https://zhuanlan.zhihu.com/p/26625249
http://www.leojuly.top/2018/11/26/Hexo-browsersync/


---