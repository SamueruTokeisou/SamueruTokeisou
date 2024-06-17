# My Personal Blog

Welcome to my personal blog! This is a simple static blog site created using Jekyll and hosted on GitHub Pages. Here, I share my journey in translation, photography, and video creation.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Deployment](#deployment)
- [License](#license)

## Introduction

This project is a personal blog site where I post articles about my work and interests. It uses Jekyll, a static site generator, to convert Markdown files into a static website.

## Installation

To get started with this project, follow these steps:

1. **Install Jekyll and Bundler**:

    ```sh
    gem install jekyll bundler
    ```

2. **Clone this repository**:

    ```sh
    git clone https://github.com/yourusername/myblog.git
    cd myblog
    ```

3. **Install dependencies**:

    ```sh
    bundle install
    ```

## Usage

To run the blog locally:

1. **Serve the site**:

    ```sh
    bundle exec jekyll serve
    ```

2. Open your browser and go to `http://localhost:4000`.

## Customization

You can customize your blog by editing the `_config.yml` file. Change the site title, description, URL, and other settings as needed.

To add a new post, create a Markdown file in the `_posts` directory. The file name should follow the format `YYYY-MM-DD-title.md`. Here is an example:

```markdown
---
layout: post
title: "Welcome to My Blog"
date: 2024-06-17
categories: introduction
---

Welcome to my personal blog! Here, I will share my journey in translation, photography, and video creation.

Deployment
To deploy your blog to GitHub Pages:

Create a new repository on GitHub.

Push the local repository to GitHub:

sh
复制代码
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/myblog.git
git push -u origin master
Configure GitHub Pages:

Go to the repository settings on GitHub.
Scroll down to the "GitHub Pages" section.
Select the master branch as the source.
Your blog should be available at https://yourusername.github.io/myblog after a few minutes.
License
This project is licensed under the MIT License. See the LICENSE file for more details.

shell
复制代码

### 文件和目录结构

在你的项目目录中，应该有以下基本文件和目录：

myblog/
├── _config.yml
├── _posts/
│ └── 2024-06-17-welcome-to-my-blog.md
├── _layouts/
├── _includes/
├── _site/
├── Gemfile
├── Gemfile.lock
└── README.md

yaml
复制代码

### `_config.yml`

以下是一个基本的`_config.yml`文件示例：

```yaml
title: My Personal Blog
description: A blog about translation, photography, and video creation.
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://yourusername.github.io" # the base hostname & protocol for your site
twitter_username: your_twitter_username
github_username: your_github_username
theme: minima
示例文章
在_posts目录中创建一个示例文章2024-06-17-welcome-to-my-blog.md：

markdown
复制代码
---
layout: post
title: "Welcome to My Blog"
date: 2024-06-17
categories: introduction
---

Welcome to my personal blog! Here, I will share my journey in translation, photography, and video creation.
完整的步骤总结
在GitHub上创建一个新仓库，如myblog。
克隆仓库到本地：
sh
复制代码
git clone https://github.com/yourusername/myblog.git
cd myblog
创建上述的文件和目录结构。
安装Jekyll和Bundler：
sh
复制代码
gem install jekyll bundler
安装依赖：
sh
复制代码
bundle install
初始化Jekyll项目（确保在myblog目录中）：
sh
复制代码
jekyll new . --force
将更改提交到GitHub：
sh
复制代码
git add .
git commit -m "Set up Jekyll blog"
git push origin master
