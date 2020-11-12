# Getting Started with VSCode, Markdown, and LaTex

### Objective
The objective of this document is to introduce VSCode, Markdown, and LaTex for Georgia Tech ECE students. By the end of this document, you will be able to install and configure VSCode, format a document using both VSCode and LaTex using common commands.

### Background
When I started ECE3057, I was asked to complete all of my lab documents using LaTex and Markdown. Having never used either languages, I was tasked with learning both the content for the class and how to setup my environment and format my documents using Markdown and LaTex.

I have created this document in hopes that it will help future students navigate Markdown and LaTex without having to search all over to find examples. This document will also as a cheat sheet for when students forget the commands they need.


# Table of Contents
1. [Setting up VSCode](#setting-up-vscode)</li>
2. [Markdown](#markdown)<br>
2.1 [Common Text Formats](#common-text-formats)<br>
2.2 [Headers](#headers)<br>
2.3 [Bold and Italics](#bold-and-italics)<br>
2.2 [Code](#code)<br>
2.3 [Tables](#tables)<br>
2.4 [Images](#images)<br>
2.5 [Equations](#equations)<br>
2.6 [Citations](#citations)<br>
3. [LaTex](#LaTex)<br>
3.1 [Common Text Formats](#common-text-formats-1)<br>
3.2 [Headers](#headers-1)<br>
3.3 [Bold and Italics](#bold-and-italics-1)<br>
3.2 [Code](#code-1)<br>
3.3 [Tables](#tables-1)<br>
3.4 [Images](#images-1)<br>
3.5 [Equations](#equations-1)<br>
3.6 [Citations](#citations-1)<br>

## Setting Up VSCode
//install here

After you have installed VSCode, I recommend installing the following extensions.

<p align="center">"Mardown PDF"</p>

Once installed, there are two key features you will want to know how to access.

Preview
Since you will want to see what your out looks like before you export to PDF, you will want to open the preview window.

- First press **CTL+SHIFT+P** and type "**Markdown: Open Preview to the Side**" and hit enter. This will open a window for you to the side that will show all of your formatted text as you type it.

Export to PDF
Once you are done writing your document, you will want to export that document, this can be done using

- First press **CTL+SHIFT+P** and type "**Markdown PDF: Export (pdf)**" and hit enter. Once the export is complete, you will have a PDF version of your document in the same directory as your Markdown file.

//Latex Workshop here

## Markdown
### Common Text Formats
**Headers**
Mardown offers a very easy syntax for creating headers ranging from size 1-6.

Typing `# Heading 1` produces:

# Heading 1

Typing `# Heading 2` produces:

## Heading 2

Typing `# Heading 3` produces:

### Heading 3

Typing `# Heading 4` produces:

#### Heading 4

Typing `# Heading 5` produces:

##### Heading 5

Typing `# Heading 6` produces:

###### Heading 6

Headings can also be used to create a table of context with clickable links to help users navigate your documents. For Example `[Heading 1](#heading-1)` will produce this link [Heading 1](#heading-1) which will take the user back to the header "Heading 1".

#### Bold and Italics

As with many documents, you may need to italicize or bold portions of your document.

Italicizing text can be done by placing `*` on each side of the text you want italicized.
- For example, `*Italicizing this is easy!*` generates *Italicizing this is just as easy!*.

Bolding text can be done by placing `**` on each side of the text you want bolded.
- For example, `**Bolding this is just as easy!**` generates **Bolding this is easy**.

Bolding and Italicizing text can be done by placing `***` on each side of the text you want bolded and italicized.
- For example, `***Bold and Italicized for the win!***` generates ***Bold and Italicized for the win!***.

#### Line Breaks and Indentions

You will inevitably find that Markdown does not always add a line break or indention where you are expecting them.

To create a line break at any point in your text, add `<br`.
- For example, `break here <br> please` generates <br>
break here <br> please

### Code

In engineering, it is not uncommon to include code blocks in your documents.

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

Admittedly, this is not very useful for large tables of data. There are plenty of webistes that you can visit that will allow you to upload csv files and will generate the necessary Markdown syntax to display your table. I would recommend the site 'https://www.tablesgenerator.com/markdown_tables'.

### Images

Images in lab reports are almost always a necessity.

For images hosted on a website, you can use the image address directly.
- For example, `![Image](https://blog.planview.com/wp-content/uploads/2017/12/cloud-750x400-750x400.jpg "random image")` generates <br>

![Image](https://blog.planview.com/wp-content/uploads/2017/12/cloud-750x400-750x400.jpg "random image")

For images that are located on your local computer, you can add teh image by using it's relative path.
- For example, `![Image2](/imgs/cover.jpg "cover image")` generates <br>

![Image2](/imgs/cover.jpg "cover image")

### Equations

Unfortunatley, Markdown does not have a direct method for adding equations or mathmatics symbols. Markdown does, however, offer direct HTML support which does allow for adding math symbols. Though Markdown equations do not look as nicely formatted as LaTex equations, they do work in a pinch.
- For example, `h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x` generates <br>

h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

A comprehensive list of HTML supported symbols can be found here, https://www.toptal.com/designers/htmlarrows/math/. You will want to use the "HTML ENTITY" code when using Markdown.

### Citations

## LaTex
### Common Text Formats
#### Headers
Stuff about Headers
#### Bold and Italics
Stuff about bold and italics
### Code
Stuff about adding code
### Tables
### Images
### Equations
 h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x
### Citations
