---
layout: default
title: Transcription Guide
permalink: docs/transcription
docs_number: 3
---

# Transcription Guide

**This page is a work in progress.**

{:toc}

# Materials concerns (copyright, etc.)?

## Optical Character Recognition (OCR) Software

Many scanned and digitized materials exist as PDFs, TIFFs, or other types of images. You can transcribe materials by hand, looking at the image and typing it word-for-word; or, you can leverage Optical Character Recognition (OCR)—a technology that converts an image of text into a machine-readable text format—to get a rough version of the text, and then you can go through the rough version to add, edit, and fix things the OCR software missed. 

No OCR tool is perfect, and the best tool for your purposes will vary a lot on the materials you have. The University of Pittsburgh has a fantastic [Optical Character Recognition LibGuide](https://pitt.libguides.com/ocr/intro) about OCR, including [OCR best practices](https://pitt.libguides.com/ocr/bestpractices), a general overview of what the process looks like, and a [list of out-of-the-box tools](https://pitt.libguides.com/ocr/outoftheboxtools) that do OCR. We've also included a comparison of some common OCR tools in the table below (including some options that often fly under the radar).

**Regardless of what tool you use, you will need to check and correct the text afterward.** The editing process can be pretty labor intensive, depending on the quality of the original scans and the amount of material you plan to transcribe. We recommend starting with just a few documents and taking them all the way through the process—scanning, transcribing, and editing—to get a feel for what works best. Then, you can go back and process the rest of your documents in a streamlined, standardized fashion.

### OCR Tool Comparison Chart
|  | Free | Batch processing | Size limit | Instructions/guides | Example output (original doc here) |
| --- | --- | --- | --- | --- | --- |
| Adobe Export PDF online* | No | Yes |  | Official guide | ocr-adobeweb.docx |
| newocr.com(checkbox for multi-column) | Yes | No |  | Homepage | ocr-newocr.dococr-newocr.txt (Plain text option) |
| ABBYY FineReader PDF | No | ? | ? | Homepage | Requires signup |
| Google Chrome (open file, select all and copy/paste) | Yes | No | - |  | ocr-chromecopy.docx |
| Adobe Acrobat DC“Edit Text” function“Export as” function | No | Yes | - | (Separate functions)“Edit text”“Export as” | ocr-adobeedit.docxocr-adobeexport.docx |
| Firefox (open file, select all and copy/paste) | Yes | No | - |  | ocr-firefoxcopy.docx |
| Google Drive (web) | Yes | No | 2 MB | Official guide | ocr-googledrive.docx |
| CopyFish |  |  |  | Copyfish docs |  |
| Transkribus (handwriting) | Y+N |  | 500 credits | Homepage | Requires signup |

## Transcribing 

### Transcribing and Editing Files Using GitHub

GitHub is great for file storage because of its versioning capabilities. But did you know that GitHub has a built-in file editor you can use right in your browser, as well? [GitHub's web-based editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor#opening-the-githubdev-editor) allows you to edit files and commit changes to your repository without having to install additional software or learn command line tools.

You can open the editor any time you are viewing your repository by pressing `.` (or `>` to open it in a new broser tab).

If you want to pull, edit, commit, and push files using your computer, you can install [GitHub Desktop](https://desktop.github.com/download/) on your computer and learn how to use it from the official [GitHub Desktop documentation](https://docs.github.com/en/desktop). You can also just use plain ol' reliable git, if you prefer.

### Metadata

Unless you directly specify metadata other than title (Author, date, etc) it will not appear for items in the metadata for the page and so will not be available for harvesters or citation programs (like Zotero).

In order to add this, you will either need to define it in the frontmatter of each page or add the values in the `_config.yml` file. Frontmatter is a better approach if every item might be different, while the config is useful if an entire folder share the same values. 

- `title:` If you have a markdown header at the top of your file, that will be taken as the "title" for the page. if you would like to set a different title, you can do so using the `title:` value
- `creator:` (look up how this would work for multiple values)
- `contributor:` contributors to the digital file, transcribers, encoders, etc.
- `published_date:` (look to see how this would work)

TODO: figure out other metadata that would need to be added to make different doc types save correctly in zotero, etc.

## TEI/XML

If you would like to work with files encoded according to the [Text Encoding Initiative Guidelines](https://tei-c.org/guidelines/), check out the [TEI Guide](https://recoveryhub.github.io/edition_template/docs/config).