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
