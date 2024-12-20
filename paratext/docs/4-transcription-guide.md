---
layout: paginate
title: Transcription Guide
permalink: documentation/transcription
category: documentation
---

# Transcription Guide

## Optical Character Recognition (OCR) software

Many scanned and digitized materials exist as PDFs, TIFFs, or other types of 
images. You can transcribe materials by hand, looking at the image and typing 
it word-for-word; or, you can leverage Optical Character Recognition (OCR)—a 
technology that converts an image of text into a machine-readable text format—to 
get a rough version of the text, and then you can go through the rough version 
to add, edit, and fix things the OCR software missed. 

No OCR tool is perfect, and the best tool for your purposes will vary a lot on 
the materials you have. The University of Pittsburgh has a fantastic 
[Optical Character Recognition LibGuide](https://pitt.libguides.com/ocr/intro) 
about OCR, including 
[OCR best practices](https://pitt.libguides.com/ocr/bestpractices), a general 
overview of what the process looks like, and a 
[list of out-of-the-box tools](https://pitt.libguides.com/ocr/outoftheboxtools) 
that do OCR. We've also included a comparison of some common OCR tools in the 
table below (including some options that often fly under the radar).

**Regardless of what tool you use, you will need to check and correct the text 
afterward.** The editing process can be pretty labor intensive, depending on the 
quality of the original scans and the amount of material you plan to transcribe. 
We recommend starting with just a few documents and taking them all the way 
through the process—scanning, transcribing, and editing—to get a feel for what 
works best. Then, you can go back and process the rest of your documents in a 
streamlined, standardized fashion.

### OCR tool comparison chart
|  Tool | Free | Batch processing | Size limit | Instructions/guides | Example output (original doc here) |
| ------- | ------- | ------- | ------- | ------- | ------- |
| Adobe Export PDF online* | No | Yes |  | Official guide | ocr-adobeweb.docx |
| newocr.com(checkbox for multi-column) | Yes | No |  | Homepage | ocr-newocr.dococr-newocr.txt (Plain text option) |
| ABBYY FineReader PDF | No | ? | ? | Homepage | Requires signup |
| Google Chrome (open file, select all and copy/paste) | Yes | No | - |  | ocr-chromecopy.docx |
| Adobe Acrobat DC“Edit Text” function“Export as” function | No | Yes | - | (Separate functions)“Edit text”“Export as” | ocr-adobeedit.docxocr-adobeexport.docx |
| Firefox (open file, select all and copy/paste) | Yes | No | - |  | ocr-firefoxcopy.docx |
| Google Drive (web) | Yes | No | 2 MB | Official guide | ocr-googledrive.docx |
| CopyFish |  |  |  | Copyfish docs |  |
| Transkribus (handwriting) | Y+N |  | 500 credits | Homepage | Requires signup |

## File creation and naming

When you create your Markdown and/or TEI transcriptions, decide early what naming 
scheme you will use to keep your files organized and unique. Depending on the 
complexity of your project, you may want to use a different scheme than the 
following; however, the naming scheme used in the template's examples create a
foundation for projects large *and* small, as it allows for future expansion 
should a small project continue to grow.

If you followed our 
[Getting Started](https://recoveryhub.github.io/edition_template/documentation/setup) 
guide, you most likely decided on a filename prefix related to your project 
name. If not, see the 
[Naming your project](https://recoveryhub.github.io/edition_template/documentation/setup#naming-your-project) 
section on that page.

## File names

Every file in your edition **must** have a unique filename, regardless of the 
file extension. In other words, if you have a Markdown file called 
`example.00001.md`, *do not name any of your TEI files* `example.00001.xml`. 

**Bad**: `example.00001.md`, `example.00001.xml`
**Good**: `example.00001.md`, `example.00002.xml`

### Single-genre editions

Text files should begin with the edition prefix and then have a padded number that 
starts with zeroes, e.g. `00001`. The length of the padding number is up to you, 
but we recommend erring on the longer side. Using 5 digits, for example, allows 
you to have 99,999 files that will always be correctly ordered when sorted by 
name (starting at `00001` and going as high as `99999`). We separate these with 
a period (`.`) to aid readability:

`file prefix` + `.` + `padded number` + `file extension`
e.g.
`ed1.00005.xml`

Note that it does not matter what numbers you choose for each file, as long as 
all the filenames are unique; they do not need to be consecutive numbers.

### Editions with multiple genres

Because the example files in this template represent different categories or 
genres of source materials, we use a slightly more detailed naming scheme. 
In addition to the file prefix, there is a two-letter code for the file's 
genre/category (`bk` for books, `cr` for correspondence,`pm` for poems, `pr` 
for periodicals), and—specific to book chapters—the abbreviation `ch` for 
chapter and a 3 digits that indicate the chapter number. 

All together, the formula we've chosen for file naming is:

`file prefix` + `.` + `genre code` + `padded number` + `file extension (.md or .xml)`
e.g.
`ed1.cr00002.xml`

With the additional coding for book chapters, it becomes:

`file prefix` + `.` + `genre code (bk)` + `padded number` + `.` + `chapter code (ch)` + `chapter number code` + `file extension (.md or .xml)`
e.g. 
`ed1.bk00001.ch001.md`

If you are naming files according to genre, it's okay to start with `00001` for 
every genre. In that case, you might have filenames like `ed1.cr00004.xml` and 
`ed1.pm00004.xml`, and that won't cause any problems.

### Why are there files in this template that don't fit the file naming scheme?

The transcriptions that make up the body of the edition use the file naming 
scheme described above, but Markdown files that are paratext (e.g. essays, 
documentation, etc.) or website pages (e.g. home, about, etc.) don't need to be 
named that way.

## Transcribing Files in Markdown

Information about encoding files in Markdown is available in our 
[Markdown Guide](https://recoveryhub.github.io/edition_template/documentation/markdown).

## Transcribing Files in TEI

Information about encoding files in TEI is available in our 
[TEI Guide](https://recoveryhub.github.io/edition_template/documentation/tei).

### Transcribing and Editing Files Using GitHub

GitHub is great for file storage because of its versioning capabilities. But 
did you know that GitHub has a built-in file editor you can use right in your 
browser, as well? [GitHub's web-based editor](https://documentation.github.com/en/codespaces/the-githubdev-web-based-editor#opening-the-githubdev-editor) allows you to edit 
files and commit changes to your repository without having to install additional 
software or learn command line tools.

You can open the editor any time you are viewing your repository by pressing `.` 
(or `>` to open it in a new broser tab).

If you want to pull, edit, commit, and push files using your computer, you can 
install [GitHub Desktop](https://desktop.github.com/download/) on your computer 
and learn how to use it from the official 
[GitHub Desktop documentation](https://documentation.github.com/en/desktop). 
You can also just use plain ol' reliable git, if you prefer.

### Metadata

This template uses [YAML Front Matter](https://jekyllrb.com/docs/front-matter/) 
to record metadata for each file. In order to work, front matter must be the 
first thing in the file, must be valid YAML (if you're following the example 
files, you'll be fine), and must be between triple-dashed lines. For example:

```
layout: about
title: About Us
```

Though front matter is the technical name, we'll use the term metadata instead 
of front matter throughout the rest of this guide, since it makes more sense in 
the language of digital editions.

If you leave a metadata field blank, it  will not appear in the metadata for 
the page and thus will not be available for harvesters or citation programs 
(like Zotero).

- `title:` If you have a Heading 1 at the top of your file (see the [Headings section of our Markdown guide]() for more information), that will be taken as the "title" for the page. if you would like to set a different title, 
you can do so using the `title:` value.
- `creator:` (look up how this would work for multiple values)
- `contributor:` contributors to the digital file, transcribers, encoders, etc.
- `published_date:` (look to see how this would work)

TODO: figure out other metadata that would need to be added to make different doc types save correctly in zotero, etc.

## TEI/XML

If you would like to work with files encoded according to the [Text Encoding Initiative Guidelines](https://tei-c.org/guidelines/), check out the [TEI Guide](https://recoveryhub.github.io/edition_template/documentation/site-config).