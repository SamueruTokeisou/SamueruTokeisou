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
