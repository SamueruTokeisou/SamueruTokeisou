# 我的个人博客 | My Personal Blog

欢迎来到我的个人博客！这是一个使用Jekyll创建的简单静态博客网站，托管在GitHub Pages上。在这里，我分享了我的翻译、摄影和视频创作之旅。

Welcome to my personal blog! This is a simple static blog site created using Jekyll and hosted on GitHub Pages. Here, I share my journey in translation, photography, and video creation.

## 目录 | Table of Contents

- [简介 | Introduction](#简介--introduction)
- [安装 | Installation](#安装--installation)
- [使用 | Usage](#使用--usage)
- [定制 | Customization](#定制--customization)
- [部署 | Deployment](#部署--deployment)
- [许可证 | License](#许可证--license)

- Typing SVG
开源字体一览（表格版）
开源字体一览（图文版）

Readme Card

个人博客 / Blog 试行 / Beta
永硕Ｅ盘 / YsEpan
外字初步整理一览表
CJK 字体 Magisk 模块模板
打赏 / Donate

关注方式 / Follow
Telegram Telegram 频道 Facebook
微信公众号 微博 哔哩哔哩
酷安 即刻 少数派
小红书 站酷

电子邮箱 / E-Mail
  

## 简介 | Introduction

这是一个个人博客网站，我在这里发布关于我的工作和兴趣的文章。它使用Jekyll，一个静态网站生成器，将Markdown文件转换为静态网站。

This project is a personal blog site where I post articles about my work and interests. It uses Jekyll, a static site generator, to convert Markdown files into a static website.

## 安装 | Installation

按照以下步骤开始使用此项目：

To get started with this project, follow these steps:

1. **安装Jekyll和Bundler | Install Jekyll and Bundler**:

    ```sh
    gem install jekyll bundler
    ```

2. **克隆此仓库 | Clone this repository**:

    ```sh
    git clone https://github.com/yourusername/myblog.git
    cd myblog
    ```

3. **安装依赖 | Install dependencies**:

    ```sh
    bundle install
    ```

## 使用 | Usage

本地运行博客：

To run the blog locally:

1. **启动站点 | Serve the site**:

    ```sh
    bundle exec jekyll serve
    ```

2. 打开浏览器并访问`http://localhost:4000`。

    Open your browser and go to `http://localhost:4000`.

## 定制 | Customization

你可以通过编辑`_config.yml`文件来定制你的博客。根据需要更改站点标题、描述、URL等设置。

You can customize your blog by editing the `_config.yml` file. Change the site title, description, URL, and other settings as needed.

添加新文章，请在`_posts`目录中创建一个Markdown文件。文件名应遵循`YYYY-MM-DD-title.md`格式。例如：

To add a new post, create a Markdown file in the `_posts` directory. The file name should follow the format `YYYY-MM-DD-title.md`. Here is an example:

```markdown
---
layout: post
title: "欢迎来到我的博客 | Welcome to My Blog"
date: 2024-06-17
categories: introduction
---

欢迎来到我的个人博客！在这里，我将分享我的翻译、摄影和视频创作之旅。

Welcome to my personal blog! Here, I will share my journey in translation, photography, and video creation.


部署 | Deployment
将博客部署到GitHub Pages：

To deploy your blog to GitHub Pages:

在GitHub上创建一个新的仓库 | Create a new repository on GitHub。

将本地仓库推送到GitHub | Push the local repository to GitHub:

sh
复制代码
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/myblog.git
git push -u origin master
配置GitHub Pages | Configure GitHub Pages:

转到GitHub上的仓库设置。

滚动到"GitHub Pages"部分。

选择master分支作为源。

几分钟后，你的博客应该会在https://yourusername.github.io/myblog上线。

Go to the repository settings on GitHub.

Scroll down to the "GitHub Pages" section.

Select the master branch as the source.

Your blog should be available at https://yourusername.github.io/myblog after a few minutes.

许可证 | License
此项目是MIT许可证的授权下获得的。详情请参阅LICENSE文件。

This project is licensed under the MIT License. See the LICENSE file for more details.

shell
复制代码

### 项目结构和配置

确保你的项目目录结构如下：

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

一个基本的`_config.yml`文件示例如下：

```yaml
title: My Personal Blog
description: A blog about translation, photography, and video creation.
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://yourusername.github.io" # the base hostname & protocol for your site
twitter_username: your_twitter_username
github_username: your_github_username
theme: minima
文章示例
在_posts目录中创建一个示例文章2024-06-17-welcome-to-my-blog.md：

markdown
复制代码
---
layout: post
title: "欢迎来到我的博客 | Welcome to My Blog"
date: 2024-06-17
categories: introduction
---

欢迎来到我的个人博客！在这里，我将分享我的翻译、摄影和视频创作之旅。

Welcome to my personal blog! Here, I will share my journey in translation, photography, and video creation.
添加语言切换按钮
为了在你的博客中添加语言切换按钮，你需要修改布局文件并添加一些JavaScript。

修改布局文件：

在_layouts目录中，找到default.html文件并添加语言切换按钮。以下是一个示例：

html
复制代码
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ page.title }}</title>
  <link rel="stylesheet" href="{{ '/assets/main.css' | relative_url }}">
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="{{ site.baseurl }}/">Home</a></li>
        <li><a href="{{ site.baseurl }}/about/">About</a></li>
        <!-- Language switch buttons -->
        <li><a href="#" id="lang-en">English</a></li>
        <li><a href="#" id="lang-zh">中文</a></li>
      </ul>
    </nav>
  </header>
  <main>
    {{ content }}
  </main>
  <footer>
    <p>© 2024 My Personal Blog</p>
  </footer>
  <script>
    document.getElementById('lang-en').addEventListener('click', function() {
      document.documentElement.lang = 'en';
    });
    document.getElementById('lang-zh').addEventListener('click', function() {
      document.documentElement.lang = 'zh';
    });
  </script>
</body>
</html>
添加样式：

确保你有一个样式表文件（如main.css）以便进行基本的样式调整。

创建双语内容：

在创建文章时，确保包含中英文内容。例如：

markdown
复制代码
---
layout: post
title: "欢迎来到我的博客 | Welcome to My Blog"
date: 2024-06-17
categories: introduction
---

欢迎来到我的个人博客！在这里，我将分享我的翻译、摄影和视频创作之旅。

Welcome to my personal blog! Here, I will share my journey in translation, photography, and video creation.
这样，你的博客将支持中英文双语内容，并提供语言切换按钮。你可以根据需要进一步定制和美化博客。
