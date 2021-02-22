---
title: Making Teenytek.com
permalink: /blog/making-teenytek/
date: 2021-02-05
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Making Teenytek.com
tags:
  - posts
---

# Making TeenyTek.com

TeenyTek.com was originally a learning project for me to learn how to use Eleventy and Node.js to maintain a much larger site built by me and my father, FarmerFrog.org. My father was the chief architect of the Farmer Frog Website, as the high school web development team did not have the knowledge or experience to rebuild the original site in the required timeframe. In order to compensate for the partial removal of the learning curve, my father recommended that my team and I build our own blog pages to practice using html, nunjucks, and css. The current iteration of the Farmer Frog website that we have been working on since September of 2020 uses so little javascript that we are not being required to use javascript, but I will most likely implement some javascript in the future since our client is already planning out features.

Eleventy is a static site generator that takes layouts built in html and nunjucks and converts content in markdown files into html and creates pages in a distribution folder. It helps keeps things extremely simple and easy to use and maintain, and is very compact since individual layouts can cover the needs of most pages. For example, The TeenyTek Website is build largely around a singular base layout that puts in a header and a footer. There are only four unique layouts used on the entire website, as well as four partial layouts for the header and the footer.

Eleventy also allows you to open the website you build on localhost instance to see how things will look on a web browser, allowing for quick and easy modification of styling or content. You can also update localhost instance live by saving the file without having to shut down the localhost instance.

TeenyTek is hosted for free by GitHub. Compared to other web hosting services such as Amazon AWS (used for Farmer Frog), GitHub is extremely simple to use, and I was able to set up my site in about 10 minutes after I created the proper forks. Github has a strange feature that requires you to put your page into a branch called gh-pages before you can push the site to a live site, and you can only put files one folder deep inside of a docs folder. I had to rename my documentation folder from docs to documentation in order to use GitHub web hosting, but GitHub will automatically aquire an SSL certificate for your site, even if you are using a custom domain. All you have to do is point your domain to your GitHub public access point, and GitHub will handle most of the work required to upload to AWS.

I will probably post updates of things I do to this site, but I may also include unique things I do on Farmer Frog, as that site is one of the projects I am very proud to have been a part of.