---
layout: paginate
title: Site Configuration Guide
permalink: documentation/site-config
---

# Site Configuration Guide

The Recovery Hub digital edition template allows you to configure and customize
your site through the `_config.yml` file. Most of the configuration settings in 
that file are settings you are expected to set up once and rarely edit after that. 

We have provided comments throughout `_config.yml` to explain what each setting 
does, but the documentation on this page offers a more detailed walkthrough to 
follow when you're setting up your site for the first time.

## Markdown Config

## TEI Config

To configure the display of TEI files, you should make sure the categories referenced in your TEI have been added to the `category_list` and that the following is included under `defaults:`

```
# Text (TEI)
  - scope:
      path: "_texts"
      type: texts
    values:
      layout: tei
```

TEI uses Jekyll collections, so you should also include: 

```
# To use Jekyll collections, set them up here:
collections: 
  texts:
    output: true
```

These sections have been added to the default `_config.yml` file for reference and can be removed from the file for editions that do not include TEI files. 