---
layout: default
title: Documentation
permalink: docs
docs_number: 1
---

# Recovery Hub Digital Edition Template
Welcome to the Recovery Hub for American Women Writers’ template for text-based digital editions.  This template supports the creation of digital editions using Markdown and TEI for transcriptions and GitHub Pages for publication on the web.

## About the Recovery Hub for American Women Writers

The Recovery Hub for American Women Writers supports projects recovering the 
work of women writers by providing digital access to forgotten or neglected 
texts and/or extending them with network mapping, spatial analysis, multimedia 
storytelling, innovative contextualization, and the distant reading of massive 
datasets. The Recovery Hub’s editorial framework—which includes this 
template—is designed to support scholars who want to encode recovered documents 
but who have limited experience with the digital humanities. Past projects have 
included digital editions of letters, books, short fiction, and other texts as 
well as experimental projects that explore mapping, visualization, and other 
content-rich methods.

The Recovery Hub fosters collaboration, mentorship, and community-building 
among women working in the digital humanities while seeking feminist and 
decolonial approaches to the creation, curation, design, sharing, and archiving 
of digital content. To learn more, visit the 
[Recovery Hub for American Women Writers website](https://recoveryhub.siue.edu/).

## Technical Information

- [GitHub Pages](https://github.com/github/pages-gem) and its [dependencies](https://pages.github.com/versions/), including [Jekyll](https://github.com/jekyll/jekyll)
- TEI in HTML5 Custom Elements based on [CETEIcean](https://github.com/TEIC/CETEIcean)
- Recovery Hub theme based on [Minima](https://github.com/jekyll/minima) version [2.5.1](https://github.com/jekyll/minima/releases/tag/v2.5.1)
- [jQuery 3.7.1 slim build](https://jquery.com/download/)
- [Fancybox](https://github.com/fancyapps/fancybox) jQuery lightbox gallery

## Getting Started

[GitHub](https://github.com/) is a free, open-access resource that stores files 
that can run a website; it can also host that website thanks to a feature called 
[GitHub pages](https://docs.github.com/pages/). 

If you don't have a GitHub account, follow the instructions for 
[Creating an account on GitHub](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github).

To get started with your own edition, click the "Use this template" button 
above to make a copy on your own GitHub account. For detailed instructions, 
see [Creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) in GitHub's official documentation.

Our recommendations for options on the "Create a new repository" page:
- Leave **Include all branches** unchecked. You won't need all the edition_base branches, just the default one.
- For **Owner**, it's okay to leave your personal account selected unless this edition should belong to a GitHub organization; if the latter, change **Owner** to your organization.
- Your **Repository name** should be short but memorable. The name cannot contain spaces, so we recommend using underscores (for example, `baker_digital_edition`).
- The **Description** is optional. You can always add or change it later.
- Whether your repository starts out as **Public** or **Private** is up to you. Either way, people will not be able to make changes without your approval. If the repository is **Private**, only people you add as members will be able to see that it exists (to learn how to add members, see [Inviting Collaborators to a personal repository](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository) in GitHub's documentation). Many people prefer to make their repository **Private** initially; just be aware that you will have to go into your settings later and change your repository to **Public** before you can publish your edition with GitHub pages.

## Folder Structure

The folders you will primarily use are:
- `docs`, which is for documentation.
- `items`, which is where your transcriptions will go when they are ready to publish. You will copy your ready-to-publish Markdown-encoded documents (`.md`) here manually.
  - If you are working with multiple genres, use the subfolders in `items` to organize your files by genre. The sample files in the template are organized by `books`, `periodicals`, and `poems`.
- `source`, which is where you'll store the following:
  - The `drafts` folder can be (re)organized to your liking. We recommending organizing them by file type (e.g. `markdown` or `tei`). In this sample template, we've also organized the Markdown drafts by genre. Both are optional.
  - The `tei` folder is where you will place your ready-to-publish TEI-encoded documents (`.xml`). 
  - The `source` folder also contains a Ruby script named `tei_to_md.rb`, which you can run locally to programmatically create Markdown files that correspond to your TEI files. You may also create the Markdown files by hand based on the examples in the `_texts` folder (see below).
- `_texts`, which is the folder that will hold the Markdown files that correspond to your TEI files. You can create these files using the `tei_to_md.rb` script included in the `source` folder, if you have Ruby installed on your computer. You can also create the files manually.
- `items`, which is where your transcriptions will end up when they are published.
- If you have images to display on your site, you can use the `assets/images` folder to organize them. The home page banner image that the template uses is `assets/images/recovery-hub-banner.jpg.` To replace it with a custom banner image, follow the instructions under [Configuring your digital edition](https://recoveryhub.github.io/edition_template/docs/config).

Folders beginning with an underscore (`_includes`, `_layouts`, etc.) contain the 
files for the Jekyll site and theme. 



## Transcription and editing

For detailed documentation on transcribing sources, organizing files, and 
readying your edition for publishing online, see our 
[Transcription tutorial](https://recoveryhub.github.io/edition_template/docs/transcription).


## Configuring your site

This template facilitates customizations through the site's `_config.yml` file. 
The `_config.yml` file contains settings that affect your whole site. 
Most are settings you are expected to set up once and rarely edit after that. 
A detailed guide to the settings and options in this file can be found in our 
[Configuring your site](https://recoveryhub.github.io/edition_template/docs/config) 
tutorial.

## Publishing your site with GitHub Pages

To publish, enable GitHub Pages by going to your repository's settings, 
clicking "Pages" in the left sidebar, choosing your branch as the source, and 
clicking save. Step-by-step instructions are available in GitHub's official documentation, 
[Configuring a publishing source for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site). Publication may take a couple of minutes. Once your site is published, the URL will be visible under "About" when you view 
your repository on GitHub.

**Your repository must be public before it can be published with GitHub Pages.** 
If your repository is currently private, [change your repository's visibility](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility) to public.

In order for links to work, you will then need to change your `_config.yml` file 
with the values of this new URL. 

**Example:** if your URL is, for instance, 
`https://recoveryhub.github.io/your_edition/`, 
then these will be your values (note the slash placement): 

```
baseurl: "/your_edition"
url: "https://recoveryhub.github.io/"
```

Once GitHub regenerates your pages (it can take up to a couple of minutes but 
is usually pretty quick), you can see your site.


























[Jekyll](https://github.com/jekyll/) is a platform that helps you create a static website from plaintext (for more on plaintext and other related terms, see our Tech Terms Glossary). Static websites are different from dynamic websites (like those made on Wordpress and Omeka) because dynamic websites pull information from a database to fill the webpage content. Jekyll sites can be written completely by users or can use HTML templates that Jekyll helps provide.

If you need to look up documentation on working with Jekyll specifically, the current docs on jekyllrb.com will not always match what you are working with since they are for a newer version. Looking for the page you need in the [Jekyll GitHub repo at the 3.9.5 release tag](https://github.com/jekyll/jekyll/tree/v3.9.5/docs) may help.
