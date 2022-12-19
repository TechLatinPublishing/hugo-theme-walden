---
title: "Hugo Theme Walden"
date: 2022-12-17T19:03:08+08:00
draft: false
author: "Homecat"
categories: "IT Notes"
tags: ["Hugo"]
thumbnail: ""
headline: 
    enabled: true
    background: ""
---

After reading <i><b>Walden</b></i>, a collection of essays by American writer Henry David Thoreau, I was deeply influenced by his love of nature and simple living. So, I wrote this concise and clear theme for my personal website and named it Walden.

<!--more-->

## Features

Walden is a simple-structured, easy-to-use Hugo theme for personal websites.

- Responsive design
- Headline on homepage
- Thumbnail for post
- Personalized shortcodes
- ...

## Demo

Two ways to see the demo：

- Visit demo site: [https://genway.com.cn/hugo-theme-walden-demo/](https://genway.com.cn/hugo-theme-walden-demo/)
- View demo by clone repository from Github: [https://github.com/homecat805/hugo-theme-walden.git](https://github.com/homecat805/hugo-theme-walden.git)

    ```
    git clone https://github.com/homecat805/hugo-theme-walden.git hugo-theme-walden
    cd exampleSite
    hugo server --themesDir ../..
    ```

## Quick start

The Hugo documentation [https://gohugo.io/installation/](https://gohugo.io/installation/) describes in detail how to install on different operating systems, which will not be repeated here, the operating system related to this article is Ubuntu 22.04 LTS.

- Create the website root directory `mysite` and perform git initialization:

    ```
    mkdir mysite
    cd mysite
    git init
    git branch -m main
    ```

- Install the theme as a module to the `mysite/themes` directory of the website, and copy all the files in the `exampleSite` directory within the theme to the root directory of the website:

    ```
    mkdir themes
    git submodule add git@github.com:Homecat805/hugo-theme-walden.git themes/hugo-theme-walden
    cp -rf themes/hugo-theme-walden/exampleSite/* ./
    ```

In subsequent use, if you need to update the theme, use the following command:

```
git submodule update --remote --merge
```

## Configuration 

The configuration file for the site is `config.toml`。

- Configure baseURL: URL of user's website on the internet.

    ```
    baseURL = "https://github.com/homecat805/walden/"
    ```

- Configure theme

    ```
    theme = "hugo-theme-walden"
    ```

## Preview

Executing the command, visit `http://localhost:1313/` to preview website locally.

```
hugo server
```

## Create Site

Executing the command, the system will store all the files generated for the static website in the `mysite/public` directory, which can be accessed after uploading to the Internet.

```
hugo
```

## License

Walden is licensed under the MIT，Check the  [LICENSE](https://github.com/homecat805/hugo-theme-walden/blob/master/LICENSE) file for details.
