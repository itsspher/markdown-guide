# Headings

The amount of ```#``` used denotes the heading level.

```markdown
# Sample Heading 1
## Sample Heading 2
### Sample Heading 3
#### Sample Heading 4
##### Sample Heading 5
```

# Sample Heading 1
## Sample Heading 2
### Sample Heading 3
#### Sample Heading 4
##### Sample Heading 5

## Alternate Syntax

You can also use `=` or `-` to denote heading level 1 and 2 respectively.

```markdown
Sample Heading 1
=========

Sample Heading 2
---------
```

Sample Heading 1
=========

Sample Heading 2
---------

# Line Breaks
Two or more spaces at the end of a line, then hit return/enter.

This sentence  
should split.

# Emphasis

## Bold
```markdown
**bold**  
__bold__  
bold**in**themiddle  
```

**bold**  
__bold__  
bold**in**themiddle  

## Italics

```markdown
*italic*  
_italic_  
italic*in*themiddle  
```

*italic*  
_italic_  
italic*in*themiddle

## Both Bold and Italic

```markdown
***both***  
___both___  
both**in**themiddle  
```

***both***  
___both___  
both**in**themiddle  

## Strikethrough
```markdown
~~wrong~~ correct
```

~~wrong~~ correct

# Blockquote

```markdown
> This is a blockquoted sentence.

> Sometimes, blockquotes have multiple paragraphs.
>
> Just put a `>` in the space between the paragraphs.
>
> > You can nest blockquotes.
>
> #### Even having other markdown elements is ok in blockquotes.
> - such
> - as
> - bullets (will discuss later).
```

> This is a blockquoted sentence.

> Sometimes, blockquotes have multiple paragraphs.
>
> Just put a `>` in the space between the paragraphs.
>
> > You can nest blockquotes.
>
> #### Even having other markdown elements is ok in blockquotes.
> - such
> - as
> - bullets (will discuss later).

# Lists

## Ordered Lists

```markdown
1. This is an ordered list.
2. Very self explanatory.
4. The numbers don't have to be in order.
6. Just as long as you start with `1.`.
    1. Indents are also possible.
    2. Just do a `TAB`.
```

1. This is an ordered list.
2. Very self explanatory.
4. The numbers don't have to be in order.
6. Just as long as you start with `1.`.
    1. Indents are also possible.
    2. Just do a `TAB`.

## Unordered Lists

```markdown
- You can use a `-`.
+ You can use a `+`.
* You can use a `*`.
- You can even mix them.
  - Same as ordered lists, indentation is possible.
  - Just do a `TAB`.
```

- You can use a `-`.
+ You can use a `+`.
* You can use a `*`.
- You can even mix them.
  - Same as ordered lists, indentation is possible.
  - Just do a `TAB`.

## Task Lists

```markdown
- [x] ~~Task 1~~ done
- [ ] Task 2
- [ ] Task 3
```

- [x] ~~Task 1~~ done
- [ ] Task 2
- [ ] Task 3

## Elements in Lists

```markdown
- Say you have a list.
- I want to put stuff under this item in this list.

  So I'll `TAB` to preserve continuity, as well as  
  leave spaces above and below this sentence.

- See? Nothing out of place.
```

- Say you have a list.
- I want to put stuff under this item in this list.

  So I'll `TAB` to preserve continuity, as well as leave spaces above and below this sentence.

- See? Nothing out of place.

# Code Blocks

```markdown
This entire document is full of them.
```

This sentence has an inline `code block`.

# Images

Make sure that your images are in the same directory.

```markdown
![Optional description(in this case, a juuling cat)](image0.jpg)
```

![Optional description(in this case, a juuling cat)](image0.jpg)

# Horizontal Rules

```markdown
***

You can make a horizontal rule with three or more asterisks.

```
***

You can make a horizontal rule with three or more asterisks.

# Links

```markdown
This is a link to [GitHub](github.com "This is an optional title.").
```

This is a link to [GitHub](github.com "This is an optional title.").


## URLs and Email Addresses

```markdown
<https://www.example.com>  
<fake@example.com>
```

<https://www.example.com>  
<fake@example.com>

Links are compatible with emphasis.

# Escaping Characters

```markdown
\* Without the backslash, this would be bulleted.
```

\* Without the backslash, this would be bulleted.

# Tables

```markdown
| Header | Header 2 |
|--------|----------|
| Table | this is a table|
| The size of columns can be irregular | It doesn't matter |
```

| Header | Header 2 |
|--------|----------|
| Table | this is a table|
| The size of columns can be irregular | It doesn't matter |

## Table Alignment

```markdown
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Left align      | Center align       | Right align   |
```

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Left align      | Center align       | Right align   |

# Footnotes

```markdown
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    This is a paragraph.
```

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    This is a paragraph.

# Heading IDs {#custom-id}

```markdown
### Heading IDs {#custom-id}
```

# Definition Lists

```markdown
Definition  
: The meaning of a word.  
: The meaning of a phrase.
```

Definition   
: The meaning of a word.  
: The meaning of a phrase.

Some markdown processors might not show this correctly.

***

# Pandoc, LaTeX, and converting Markdown files into documents/slides

## Pandoc

Pandoc is magic and can be used for document conversion of all sorts.  
Pandoc and related information can be found [here](https://pandoc.org/).

## LaTex

The full installation of LaTeX is quite large, around 2 GB, if you want that, use [TeX Live](https://tug.org/texlive/).  
A smaller LaTeX is [MiKTeX](https://miktex.org/download). (Around 220 MB for Windows users, less so for OSX/Linux.)  
LaTeX allows for formatting complex math equations in Markdown documents, an example of which is this:

```markdown
$$
z \left( 1 \ +\ \sqrt{\omega_{i+1} + \zeta -\frac{x+1}{\Theta +1} y + 1}
\ \right)
\ \ \ =\ \ \ 1
$$
```

$$
z \left( 1 \ +\ \sqrt{\omega_{i+1} + \zeta -\frac{x+1}{\Theta +1} y + 1}
\ \right)
\ \ \ =\ \ \ 1
$$

A guide to LaTeX math can be found [here](https://en.wikibooks.org/wiki/LaTeX/Mathematics).

## Converting Markdown to documents

With Pandoc and LaTeX installed, simply open a terminal at the directory of the `.md` file and enter the command:

```
pandoc filename.md -o filename.pdf
```
This will produce a basic `.pdf` of your Markdown file.  
Further customization of the way the `.pdf` is compiled can be found [here](https://learnbyexample.github.io/tutorial/ebook-generation/customizing-pandoc/).  
My personal command is this, if you wish to use it:
```
pandoc filename.md -o filename.pdf --template eisvogel -V linkcolor:blue --pdf-engine=xelatex --highlight-style monochrome
```

### Eisvogel, a custom LaTeX template

I personally like to use a custom template for document compilations, so that my documents don't look like a generic *blargh*.  
Details for Eisvogel can be found [here](https://github.com/Wandmalfarbe/pandoc-latex-template).  

## Converting Markdown to slides

A guide for using Pandoc and Markdown to make slides can be found [here](http://pages.stat.wisc.edu/~yandell/statgen/ucla/Help/Producing%20slide%20shows%20with%20Pandoc.html).  
Here's some decent, non-academic-stuffy-generic looking themes.  
[Material Design by GitHub user edasubert](https://github.com/edasubert/beamerMaterialDesign)  
[Metropolis by GitHub user matze](https://github.com/edasubert/beamerMaterialDesign)  
These themes are designed to be used primarily with LaTeX, so they may not be necessarily be compatible with Markdown. Your mileage may vary.

***

# Credit where credit is due

A lot of this document is shortened versions of Markdown documentation from various sites.  
[Pandoc's Markdown](https://pandoc.org/MANUAL.html#pandocs-markdown)  
[Markdown Guide](https://www.markdownguide.org/)

***

Some of the elements in this document may break due to the template, differences in pandoc's Markdown and GitHub Markdown, or other weird reasons, apologies for that.
