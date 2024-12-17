---
layout: default
title: Site Configuration Guide
permalink: docs/config
docs_number: 2
---
# Site Configuration Guide

The Recovery Hub edition template facilitates customizations through the site’s `_config.yml` file. The `_config.yml` file contains settings that affect your whole site. Most are settings you are expected to set up once and rarely edit after that. Comments in the template `_config.yml` file should help to guide you in initial setup of that file. Below is some additional information about the `_config.yml` file. 

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