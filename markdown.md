# Markdown

- [Introduction](#introduction)
- [Installation & Setup](#installation-and-setup)
- [Examples](#examples)
    - [Headers](#headers)
    - [Paragraphs](#paragraphs)
    - [Text style](#text-style)
    - [Lists](#lists)
        - [Itemized list](#itemized-list)
        - [Enumerated list](#enumerated-list)
        - [Nested lists](#nested-lists)
    - [Code](#code)
    - [Footnote](#footnote)


<a name="introduction"></a>
## Introduction

> {link} You may be interested to read more on [wikipedia page](https://en.wikipedia.org/wiki/Markdown).

Markdown is a lightweight markup language with plain text formatting syntax. It's designed so that it can be converted to HTML and many other formats using a tool by the same name. 

Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor. As the initial description of Markdown contained ambiguities and unanswered questions, many implementations and extensions of Markdown appeared over the years to answer these issues.

<a name="installation-and-setup"></a>
## Installation & Setup

Are you kidding? You need noting to use markup language like Markdown. Open up your favourite texteditor and write some markdown ([examples](/docs/markdown#examples)), save file as `.md` and you are done.

<a name="examples"></a>
## Examples

<a name="headers"></a>
### Headers

Use hash symbol `#` to indicate that you want to make text a heading.

```
  # Big header <h1>
  ## Medium header <h2>
  ### Small header <h3>
  #### Tiny header <h4>
  ##### Never used header <h5>
```

# Big header <h1>
## Medium header <h2>
### Small header <h3>
#### Tiny header <h4>
##### Never used header <h5>

<a name="paragraphs"></a>
### Paragraphs

Paragraphs are divided by blank line.

<a name="text-style"></a>
### Text style

```
You are welcome to use **bold**, *italic*, `code`.
```

Translates into:

You are welcome to use **bold**, *italic*, `code`.

<a name="lists"></a>
### Lists

<a name="itemized-list"></a>
#### Itemized list

These lists are most common, use asterisk `*` to start itemized list

```
  * item
  * item
```

Looks like this:

  * item
  * item

<a name="enumerated-list"></a>
#### Enumerated list

Simply start with `1.` and continue numbering...

```
  1. one
  2. two
```

Looks like follwing

  1. one
  2. two

> {tip} Itemized list is better since order does not matter.

<a name="nested-lists"></a>
#### Nested lists

You are welcome to nest lists:

  * just 
    1. like
    2. this
  * example

<a name="code"></a>
### Code

Large blocks of codes start and end with three backticks ```.

```
#!/bin/sh
echo "Hello world"
```

Or with syntax higlighting for shell.

```shell
#!/bin/sh
echo "Hello world"
```

Yap documentation syntax highlights these languages:
  * markup
  * css
  * clike
  * javascript
  * apacheconf
  * batch
  * c
  * bison
  * cpp
  * git
  * go
  * haskell
  * http
  * latex
  * markdown
  * matlab
  * nginx
  * python
  * sql
  * vim
  * yaml

<a name="footnote"></a>
### Footnote

Here's a footnote [^1] example.

[^1]: Footnote text goes here.
