---
layout: default
title: Markdown Guide
permalink: docs/markdown
docs_number: 4
---

# Markdown Guide

{:toc}

## Basic terminology

Some basic terminology:

### Characters
In computing terms, a character is any letter, number, space, punctuation mark, 
or symbol. `A` is a character; `9` is a character; `?` is a character; etc.
"Character" became a familiar term for many denizens of social media thanks to 
the "character limit," that is, the max number of characters (letters, numbers, 
line breaks, symbols, etc.) allowed in a single social media post. (Lookin' at 
you, Twitter. RIP.)

### Syntax
You're probably familiar with the term "syntax" as it is used in linguistics: 
rules that govern how words and phrases are arranged to create well-formed 
sentences. Similarly, in coding and programming languages, "syntax" refers to 
the arrangement of words, symbols, and other characters to create well-formed 
code. If, in your code, the syntax is correct, that piece of code will function 
and display correctly in your end result. If your syntax is incorrect, it will 
usually display incorrectly, function incorrectly, or not display or function 
at all (and potentially "break" the page until it's fixed). If you hear someone 
say "Check your syntax," they mean proofread your code. Sometimes all it takes 
is missing a space or a symbol in your code.

### Wrap/Wrapping
When we say to wrap something with something else, like "wrap your text in 
underscores," that essentially means "put an underscore before and after your 
text," like so: `_your text_`. As you transcribe materials in Markdown, you can 
format words, paragraphs, and other elements by wrapping them with specific 
characters.

## Markdown
Markdown is lightweight "markup" language that allows users to take plain text 
and add formatting elements (headings, lists, italics, footnotes, etc.). You'll 
create your pages using Markdown files (`.md`), and GitHub Pages will display 
them as HTML pages on your site.

The [Markdown Cheat Sheet from markdownguide.org](https://www.markdownguide.org/cheat-sheet/) 
is a great page to have up while you are transcribing and editing your Markdown 
files. It's a quick-reference list of all the ways you can format things in 
Markdown, from bold and italics to footnotes and images. Rather than duplicate 
the excellent guides that accompany the Cheat Sheet here, we provide links and 
some brief annotations for things commonly used in digital editions. 

### Basic Markdown Elements

#### [Paragraphs](https://www.markdownguide.org/basic-syntax/#paragraphs-1)

Perhaps the most straightforward element in this list, paragraphs are formed 
simply by separating two lines of text with a blank line.

```
This is my first paragraph.

This is my second paragraph.
```

#### [Headings](https://www.markdownguide.org/basic-syntax/#headings)

All markdown files must have either a 
[Heading 1](https://www.markdownguide.org/basic-syntax/#headings) at the top of 
the document, or must declare a `title:` in the frontmatter. (Note: if the file 
has a `title:` in the frontmatter, it supercedes the Heading 1 and becomes the 
HTML page `<title>`, but will not replace the Heading 1 on the page.)

Page titles, section titles, and other headings must be formatted as actual 
headings, *not as bold text*. Headings are essential for accessibility on the 
web, as they allow people using assistive technologies (like a person who is 
blind using screen reader software) to understand the organization of a page 
the way a person with no visual disability would. Screen readers do not 
announce that text is bold, italicized, or in a bigger font; screen readers do 
recognize headings that are formatted correctly, however, and will announce 
them as such.

#### [Bold Text](https://www.markdownguide.org/basic-syntax/#bold) and [Italicized Text](https://www.markdownguide.org/basic-syntax/#italic)

Both asterisks (`*`) and underscores (`_`) can be used to make words or phrases 
bold and/or italicized. To italicize text, wrap it in single underscores 
(`_this_` turns into _this_) or single asterisks (`*this*` turns into *this*). 
To make text bold, wrap it in _double_ underscores or _double_ asterisks 
(`**this**` turns into **this**, and `__this__` also turns into __this__). 

**Whatever you choose to use, stay consistent.** For this tutorial, we use the 
underscore for italics (like `_this_`) and double asterisks for bold text 
(like `**this**`), since that makes it easier to visually distinguish between 
bold and italics when skimming through or proofreading a Markdown file. 
However, underscores do _not_ work within a word, so that may impact your 
decision. (For example, `a_maz_ing` simply turns into amazing—with no 
italics—while `a*maz*ing` turns into a*maz*ing with the letters *m*, *a*, and *z* 
italicized.)

**Do not use bold text as a substitute for real headings.** To learn how to 
format text as a heading, see the previous section of this page.

#### [Line breaks](https://www.markdownguide.org/basic-syntax/#line-breaks)

Use paragraphs as much as you can, unless you are, in fact, transcribing line 
breaks rather than paragraphs, and don't want the additional space that comes 
between paragraphs. Since GitHub Pages supports HTML, you can insert a line 
break using the HTML tag `<br>`.

This template for digital editions has a special system for poetry. For 
information on formatting poems or similar forms of writing, see the section on 
[Formatting poetry](#formatting-poetry) at the end of this tutorial.

#### [Superscript](https://www.markdownguide.org/extended-syntax/#superscript)

**Do NOT use superscript formatting to create footnotes.** In Markdown, 
creating a footnote (e.g. `This sentence has a relevant footnote.[ch1-ref1]`) 
automatically adds the superscript footnote number for you. You do not need to 
add the extra symbols described here.

To make a character superscript, wrap it in caret symbols (for example, 
`19^th^ century` results in 19^th^ century).

### Footnotes

[Footnotes](https://www.markdownguide.org/extended-syntax/#footnotes) allow you 
to add notes and references that will automatically appear at the bottom of the 
page[^1]. When you create a footnote, a superscript number with a link appears 
where you added the footnote reference. Readers can click the link to jump to 
the content of the footnote at the bottom of the page. 

**We highly recommend formatting your footnotes consistently across all files.** 
This is especially important if you have multiple people contributing to the 
edition, or if you have chapters of a book or other parts of a whole that 
are displayed individually in one place but displayed all together in another. 
Consistency is good practice even for simple projects, however.

#### Inserting Footnotes

To add a footnote within your text, add a caret and a **footnote ID** inside 
square brackets. 

For example: 

```
This is a paragraph with a footnote in it [^ch1-ref1]. I've chosen ch1-ref1 as the footnote ID.
```

results in:

> This is a paragraph with a footnote in it[^ch1-ref-1]. I've chosen ch1-ref1 as the footnote ID.

**The ID is not what will appear on the page.** Footnotes numbers will be 
generated automatically when you view the page (1, 2, 3, etc.). IDs can be 
numbers or words (and we recommend a standardized combination of the two), but 
they can’t contain spaces or tabs. For example, the sample book chapters in 
this template use an abbreviated chapter number + footnote number pattern for 
all footnotes, e.g. `[^ch1-ref1]`. We recommend following a similar pattern, 
but tailored to fit your project. Doing this ensures that when all the chapters 
are displayed on a single page, all the footnote IDs will be unique, and all 
the footnote links will work. If you use the same footnote IDs in every chapter 
(for example, if every chapter has a `[^1]`, `[^2]`, `[^3]`, etc. etc.), then 
when all the chapters are displayed on a single page, all footnotes formatted 
as `[^1]` will link to the same footnote.

### Adding Footnote Text

In Markdown, you don’t have to put the footnote text at the end of the document; 
you can put it anywhere except inside other elements like lists, block quotes, 
and tables. It still works fine to put them all at the end of the document, 
though. Whatever you decide, we recommend doing it consistently across all of 
your files for easier editing.

To add the text/body of the footnote, type the caret and footnote ID (like you 
just did in the body of the text) followed by a colon and the text of your 
footnote, like so: 

```
[^ch1-ref1]: Here is the text of the footnote that will appear at the end of the document.
``` 

### Other useful things you can add to your GitHub pages site with Markdown

#### Table of Contents

Github Pages will automatically display a Table of Contents to your file if you include the code `{:toc}`. The Table of Contents will link to headings in your document, so make sure to use proper hierarchy/nesting of headings.

#### [Tables](https://www.markdownguide.org/extended-syntax/#tables)
Tables are not the easiest to create and edit in Markdown. Adding a table from scratch can be rather time consuming; it's often easier to copy and paste an example table and then replace the example text inside it, or use a [Markdown table generator](https://www.tablesgenerator.com/markdown_tables).

#### [Images](https://www.markdownguide.org/basic-syntax/#images-1)

Your edition may or may not include images. If you want to include an image on a page, you'll need to place it in the Jekyll folder for images, `/assets/images`. Then, you can follow the [markdownguide.org instructions for images](https://www.markdownguide.org/basic-syntax/#images-1) to insert it into a page.





# Formatting Poetry

This digital edition template uses Markdown and CSS for a custom method of 
transcribing and displaying verses, stanzas, and indentation often used in 
poetry. Rather than inserting a line break after every verse/line, each line is 
formatted as a bullet in a bulleted list, and stanzas are separated by a blank line, like so:

```
- Stanza 1 line 1
- Stanza 1 line 2
- Stanza 1 line 3

- Stanza 2 line 1
- Stanza 2 line 2
- Stanza 2 line 3
```

If you need more space between stanzas than what is displayed by default, you 
can insert multiple HTML `<br>` tags between paragraphs to add line breaks.

```
- This is my first stanza, 
- which should have extra space 
- between it and the second stanza.

<br><br>

- This is my second stanza.
```