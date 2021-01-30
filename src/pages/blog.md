---
title: TeenyTek Blog
layout: blog-layout.njk
permalink: "/blog/{% if pagination.pageNumber > 0 %}{{ pagination.pageNumber | plus: 1 }}{% endif %}/index.html"
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
pagination:
    data: collections.posts
    reverse: true
    size: 5
    alias: posts
---