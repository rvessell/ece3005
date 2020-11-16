# Getting Started with VSCode, Markdown, and LaTex
Author: Ryan Vessell, 3rd Year Computer Engineering Student
Date: 11/16/2020

# Preface
//something here

# Table of Contents
1. [Objective](#objective)
2. [Background](#background)
3. [Setting up VSCode](#setting-up-vscode)
4. [Common Text Formats](#common-text-formats)<br>
4.1 [Headers](#headers)<br>
4.2 [Permalinks](#permalinks)<br>
4.3 [Bold and Italics](#bold-and-italics)<br>
4.4 [Line Breaks and Indentions](#line-breaks-and-indentions)<br>
4.5 [Alignment](#alignment)<br>
5. [Code](#code)<br>
6. [Tables](#tables)<br>
7. [Images](#images)<br>
8. [Equations](#equations)<br>
9. [Links](#links)<br>

### Objective
<p> The objective of this document is to introduce VSCode, and Markdown for Georgia Tech ECE students. By the end of this document, you will be able to install and configure VSCode, format a document using Markdown commands. This document is not meant to be a comprehensive list of all available Markdown commands, instead, it is meant to be a quick start guide for the commands that I have found most useful.

### Background
<p> When I started ECE3057, I was asked to complete all of my lab documents using Markdown. Having never used Markdown, I was tasked with learning both the content for the class and how to setup my environment and format my documents using Markdown.

<p> I have created this document in hopes that it will help future students navigate Markdown and VSCode without having to search all over to find examples. This document will also as a cheat sheet for when students forget the commands they need.

## Setting Up VSCode

### Installation

First, you'll need to download the VSCode installer. This can be found here https://code.visualstudio.com/download. <br>

- Once downloaded, run the installer. Read the installation agreement and then accept it. <br>

![1](https://github.com/rvessell/ece3005/blob/main/imgs/inst/1.PNG?raw=true "Agreement") <br>

- Choose your installation location, in this example, we will use the default. <br>

![2](https://github.com/rvessell/ece3005/blob/main/imgs/inst/2.PNG?raw=true "Location") <br>

- Choose the shortcut name, in this example, we will use the default. <br>

![3](https://github.com/rvessell/ece3005/blob/main/imgs/inst/3.PNG?raw=true "Shortcut") <br>

- Review any settings that you have changed and click install.<br>

![4](https://github.com/rvessell/ece3005/blob/main/imgs/inst/4.PNG?raw=true "Install") <br>

### Extension

After you have installed VSCode, the following extension is highly reocmmended. <br>

Markdown PDF<br>

- First, click on the extensions icon in VSCode. <br>

![1](https://github.com/rvessell/ece3005/blob/main/imgs/ext/1.png?raw=true "Extensions") <br>

- Next, search for Markdown PDF in the extension search bar and click the green install button. <br>

![2](https://github.com/rvessell/ece3005/blob/main/imgs/ext/2.png?raw=true "Search") <br>

Once installed, there are two key features you will want to know how to access. <br>

Preview <br>
<p> Since you will want to see what your output looks like before you export to PDF, you will want to open the preview window. <br>

- First press **CTL+SHIFT+P** and type "**Markdown: Open Preview to the Side**" and hit enter. This will open a window for you to the side that will show all of your formatted text as you type it. <br>

![Markdown Preview](https://github.com/rvessell/ece3005/blob/main/imgs/ext/preview.png?raw=true "Markdown Preview")<br>

Export to PDF <br>
Once you are done writing your document, you will want to export that document, this can be done using Markdown Export to PDF. <br>

![Markdown Export to PDF](https://github.com/rvessell/ece3005/blob/main/imgs/ext/export.png?raw=true "Markdown Export to PDF") <br>

- First press **CTL+SHIFT+P** and type "**Markdown PDF: Export (pdf)**" and hit enter. Once the export is complete, you will have a PDF version of your document in the same directory as your Markdown file. <br>

## Common Text Formats

<p> In almost every document an engineer writes, one will need to define sections, indent paragraphs, bold and or italicize some blocks of text and align objects to effectively display the information they are providing.

#### Headers
---------------------
<p> Markdown offers a very easy syntax for creating headers ranging from size 1-6.

Typing `# Heading 1` produces:

# Heading 1

Typing `## Heading 2` produces:

## Heading 2

Typing `### Heading 3` produces:

### Heading 3

Typing `#### Heading 4` produces:

#### Heading 4

Typing `##### Heading 5` produces:

##### Heading 5

Typing `###### Heading 6` produces:

###### Heading 6

#### Permalinks
---------------------
<p> Headings can also be used to create a table of context with clickable links to help users navigate your documents. For Example `[Heading 1](#heading-1)` will produce this link [Heading 1](#heading-1) which will take the user back to the header "Heading 1".

#### Bold and Italics
---------------------

<p> As with many documents, you may need to italicize or bold portions of your document.

Italicizing text can be done by placing `*` on each side of the text you want italicized.
- For example, `*Italicizing this is easy!*` generates *Italicizing this is just as easy!*.

Bolding text can be done by placing `**` on each side of the text you want bolded.
- For example, `**Bolding this is just as easy!**` generates **Bolding this is easy**.

Bolding and Italicizing text can be done by placing `***` on each side of the text you want bolded and italicized.
- For example, `***Bold and Italicized for the win!***` generates ***Bold and Italicized for the win!***.

#### Line Breaks and Indentions
---------------------

<p> You will inevitably find that Markdown does not always add a line break or indention where you are expecting them. <br>

To create a line break at any point in your text, add `<br`.
- For example, `break here <br> please` generates <br>
break here <br> please

#### Alignment
---------------------

<p> Text alignment is not something that Markdown can do, luckily, it is something that HTML can do, which is natively supported in Markdown.

<p> To center a block of text, you can add `<p align="center"></p>` to the text that you would like to center.

- For example, `<p align="center">Center this please.</p>` generates

<p align="center">Center this please.</p>

### Code
---------------------

<p> In engineering, it is not uncommon to include code blocks in your documents.

To include code portions inline with your text, place \` on each side of your code.
- For example, \`mkdir new_dir\` generates `mkdir new_dir`.

To include code blocks, usually done with larger sections of code that include line breaks, start each line of the with four spaces 
- For example<br>

for(int i = 0; i < num; ++i){
   printf("i: %d");<br>
}<br>
generates

    for(int i = 0; i < num; ++i){
        printf("i: %d");<br>
    }

### Tables
---------------------

Tables are often one of the most effective ways engineers can display data. A simple table can be created using a series of `|` symbols.
- For example <br>
`| Name 	| Age 	| Major 	|`<br>
`|-	|-	|-	|`<br>
`| George B 	| 93 	| Ceramic Engineering 	|`<br>
`| Ryan V 	| 32 	| Computer Engineering 	|`<br>

generates

| Name 	| Age 	| Major 	|
|-	|-	|-	|
| George B 	| 93 	| Ceramic Engineering 	|
| Ryan V 	| 32 	| Computer Engineering 	|

<p> Admittedly, this is not very useful for large tables of data. There are plenty of websites that you can visit that will allow you to upload csv files and will generate the necessary Markdown syntax to display your table. I would recommend the site 'https://www.tablesgenerator.com/markdown_tables'.

### Images
---------------------

<p> Images in lab reports are almost always a necessity.

For images hosted on a website, you can use the image address directly.
- For example,`![Image](https://blog.planview.com/wp-content/uploads/2017/12/cloud-750x400-750x400.jpg "random image")` generates <br>

![Image](https://blog.planview.com/wp-content/uploads/2017/12/cloud-750x400-750x400.jpg "random image")

For images that are located on your local computer, you can add the image by using it's relative path.
- For example, `![Image2](/imgs/cover.jpg "cover image")` generates <br>

![Image2](./imgs/cover.jpg "cover image")

### Equations
---------------------

<p> Unfortunately, Markdown does not have a direct method for adding equations or mathematics symbols. Markdown does, however, offer direct HTML support which does allow for adding math symbols.
- For example, `h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x` generates <br>

h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

Below are some other common symbols.

| code | symbol |
|- |- |
|`&times;` | &times; |
|`&ne;` | &ne; |
| `&plusmn;` | &plusmn; |
| `&fnof;` | &fnof; |
| `&sum;` | &sum;

<p> A comprehensive list of HTML supported symbols can be found here, https://www.toptal.com/designers/htmlarrows/math/. You will want to use the "HTML ENTITY" code when using Markdown.

## Links

VSCode Installation Files - https://code.visualstudio.com/download <br>
Table Generator - https://www.tablesgenerator.com/markdown_tables <br>
HTML Math Symbols - https://www.toptal.com/designers/htmlarrows/math/ <br>
