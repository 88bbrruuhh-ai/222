---
title: Getting Started with PagesCMS
published: true
date: 2024-01-15
author: Admin
tags: [Tech, Tutorial]
excerpt: Learn how to set up and configure PagesCMS for your static website. This comprehensive guide covers everything from basic setup to advanced configurations.
cover: /media/blog/pagescms-tutorial.jpg
---

# Getting Started with PagesCMS

PagesCMS is revolutionizing how we manage content for static websites. In this tutorial, we'll walk through setting up PagesCMS for your project.

## What is PagesCMS?

PagesCMS is an open-source Content Management System designed specifically for static site generators. It provides:

- **User-friendly Interface**: No need to edit markdown files directly
- **GitHub Integration**: Content is stored in your GitHub repository
- **Rich Media Support**: Easy image and file management
- **Flexible Configuration**: Customizable fields and content types

## Basic Setup

### 1. Install PagesCMS

First, you'll need to set up PagesCMS in your project:

```bash
npm install @pages-cms/core
```

### 2. Create Configuration

Create a `.pages.yml` file in your project root:

```yaml
media:
  input: media
  output: /media

content:
  - name: posts
    label: Blog Posts
    type: collection
    path: content/posts
    fields:
      - name: title
        label: Title
        type: string
        required: true
      - name: body
        label: Content
        type: rich-text
```

### 3. Deploy PagesCMS

Deploy PagesCMS to your preferred hosting platform and connect it to your GitHub repository.

## Advanced Features

### Custom Fields

PagesCMS supports various field types:

- **String**: Simple text input
- **Text**: Multi-line text area
- **Rich-text**: WYSIWYG editor
- **Image**: Image upload and selection
- **Date**: Date picker
- **Boolean**: Toggle switch
- **Select**: Dropdown with options

### Media Management

Configure media handling for different asset types:

```yaml
media:
  - name: images
    label: Images
    input: media/images
    output: /media/images
    categories: [image]
  - name: documents
    label: Documents
    input: media/docs
    output: /media/docs
    categories: [document]
```

## Conclusion

PagesCMS makes content management for static sites incredibly easy. With its intuitive interface and powerful configuration options, you can create a professional content management workflow in minutes.

---

*Happy content managing! 🎉*
