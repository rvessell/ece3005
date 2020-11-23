# Getting Started with VSCode, Markdown, and LaTex
Author: Ryan Vessell, 3rd Year Computer Engineering Major<br>
Institution: Georgia Institute of Technology<br>
Course: ECE 3005 - Fall 2020<br>
Date: 11/16/2020

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
---------------------
  The objective of this document is to introduce VSCode, and Markdown for Georgia Tech ECE students. By the end of this document, students will be able to install and configure VSCode, format a document using Markdown commands. This document is not meant to be a comprehensive list of all available Markdown commands, instead, it is meant to be a quick start guide for the commonly used commands.

### Background
---------------------
  In Fall 2020, ECE 3057 students were asked to complete their lab reports using Markdown. Some of the students in the course had never used Markdown before and were tasked with learning Markdown as well as the content of the course.
   
  This document was created in hopes that it will help future students navigate Markdown and VSCode without having to search through multiple resources to find examples. This document will also act as a cheat sheet when students forget the commands they need

## Setting Up VSCode

  VSCode is quickly becoming one of the most populate IDEs for developers across many popular programming languages. What makes VSCode so enticing is that it is extremely lightweight. Historically, a lightweight IDE meant a distinct lack of features. VSCode combats this notion by supporting open source extentions. The extensions range from broad programming language support to purpose built tools to achieve a singular goal.

### Installation
---------------------

  The following steps will guide those that are new to VSCode through the installation process. Since VSCode is so lightweight, the installation process is very straight forward.

- First, download the VSCode installer. The installation media can be found here https://code.visualstudio.com/download. <br>

- Once downloaded, run the installer. Read the installation agreement and then accept it. <br>

<p align="center">
  <img width="460" height="300" title="Agreement" src="https://github.com/rvessell/ece3005/blob/main/imgs/inst/1.PNG?raw=true"><br>
  Figure 1: Agreement Window
</p>

- Choose the desired installation location, in this example, the default locations were used. <br>

<p align="center">
  <img width="460" height="300" title="Location" src="https://github.com/rvessell/ece3005/blob/main/imgs/inst/2.PNG?raw=true"><br>
  Figure 2: Location Window
</p>

- Choose the shortcut name, in this example, the default names were used. <br>

<p align="center">
  <img width="460" height="300" title="Shortcut" alt="Shortcut" src="https://github.com/rvessell/ece3005/blob/main/imgs/inst/3.PNG?raw=true"><br>
  Figure 3: Shortcut Name Window
</p>

- Review any custom settings and click install.<br>

<p align="center">
  <img width="460" height="300" title="Install" src="https://github.com/rvessell/ece3005/blob/main/imgs/inst/4.PNG?raw=true"><br>
  Figure 4: Confirmation Window
</p>

### Extension
---------------------

  Several extensions were tested prior to the creation of this document, and at that time, Markdown PDF was determined to be the best choice for creating a Markdown document. For students searching for an alternative to Markdown PDF, VSCode-Pandoc is an appropriate alternative, though, it was found to be more difficult to setup and a bit more bloated than Markdown PDF. Below are the steps for installing Markdown PDF.

- First, click on the extensions icon in VSCode. <br>

<p align="center">
  <img title="Extensions" src="https://github.com/rvessell/ece3005/blob/main/imgs/ext/1.png?raw=true"><br>
  Figure 5: Extensions Menu
</p>

- Next, search for Markdown PDF in the extension search bar and click the green install button. <br>
<p align="center">
  <img width="860" height="200" title="Extensions" src="https://github.com/rvessell/ece3005/blob/main/imgs/ext/2.png?raw=true"><br>
  Figure 6: Search Menu
</p>

#### Markdown: Preview
---------------------

  Markdown is ironically, a markup language, so when a document is being written, the results are not immediately shown. Traditionally, the results are only shown once the document has been compiled. This method is time intensive and not condusive to quick document creation. Markdown PDF offers a Preview feature that allows for a realtime view of the formatting of a document. This allows the document creator to view and change formatting without having to compile between iterations. Below are the steps for using the Preview feature in Markdown PDF. <br>

- First press **CTL+SHIFT+P** and type "**Markdown: Open Preview to the Side**" and hit enter. This will open a window for you to the side that will show all of your formatted text as you type it. <br>

<p align="center">
  <img width="800" height="150" title="Extensions" src="https://github.com/rvessell/ece3005/blob/main/imgs/ext/preview.png?raw=true"><br>
  Figure 7: Markdown Preview
</p>

#### Markdown: Export PDF
---------------------

  Previewing a Markdown document is helpful, but eventually, the document will often need to be exported to a more common format, such as a PDF. Below are the steps for using the Export to PDF feature in Markdown PDF <br>

<p align="center">
  <img width="800" height="150" title="Extensions" src="https://github.com/rvessell/ece3005/blob/main/imgs/ext/export.png?raw=true"><br>
  Figure 7: Markdown Export to PDF
</p>

- First press **CTL+SHIFT+P** and type "**Markdown PDF: Export (pdf)**" and click enter. Once the export is complete, a PDF version of the document will be created in the same directory as the Markdown file. <br>

## Common Text Formats

  In almost every document an engineer writes, one will need to define sections, indent paragraphs, bold and or italicize some blocks of text and align objects to effectively display the information they are providing.

#### Headers
---------------------
  Markdown offers a very easy syntax for creating headers ranging from size 1-6.

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
  Headings can also be used to create a table of context with clickable links to help users navigate documentation. For Example `[Heading 1](#heading-1)` will produce this link [Heading 1](#heading-1) which will take the user back to the header "Heading 1".

#### Bold and Italics
---------------------

  Italics are used in technical documentation when representing variables, including titles of other texts, and introducing a new term.

Italicizing text can be done by placing `*` on each side of the text you want italicized.
- For example, `*Italicizing this is easy!*` generates *Italicizing this is just as easy!*.

Bolding text can be done by placing `**` on each side of the text you want bolded.
- For example, `**Bolding this is just as easy!**` generates **Bolding this is easy**.

Bolding and Italicizing text can be done by placing `***` on each side of the text you want bolded and italicized.
- For example, `***Bold and Italicized for the win!***` generates ***Bold and Italicized for the win!***.

#### Line Breaks and Indentions
---------------------

  Like many programming languages, Markdown does not recognize new lines as new lines and or tabs as indentions. While this is not exactly a Markdown syntax, it is an HTML symbol which is natively supported in Markdown.

To create a line break at any point in your text, add `<br`.
- For example, `break here <br> please` generates <br>
break here <br> please

To create an indention `&nbsp;` can be used.
- For example, `&nbsp; This is the beginning of a paragraph. It has more than one sentence.` generates.<br>
&nbsp; This is the beginning of a paragraph. It has more than one sentence.


#### Alignment
---------------------

  Text alignment is not something that Markdown can do, luckily, it is something that HTML can do, which is natively supported in Markdown.

<p> To center a block of text, you can add `<p align="center"></p>` to the text that you would like to center. </p>

- For example, `<p align="center">Center this please.</p>` generates 

<p align="center">Center this please.</p>

### Code
---------------------

  In engineering, it is not uncommon to include code blocks in your documents. Clearly displaying the code can be the difference between a well received document and one that is unusable.

To include code portions inline with the text, place \` on each side of the code.
- For example, \`mkdir new_dir\` generates `mkdir new_dir`.

To include code blocks, usually done with larger sections of code that include line breaks, start each line of the code with four spaces.
- For example<br>

for(int i = 0; i < num; ++i){<br>
   printf("i: %d");<br>
}<br>
generates

    for(int i = 0; i < num; ++i){
        printf("i: %d");<br>
    }

### Tables
---------------------

  Tables are often one of the most effective ways engineers can display data.

A simple table can be created using a series of `|` symbols.
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

  Admittedly, this is not very useful for large tables of data. There are plenty of websites that will allow the upload csv files and will generate the necessary Markdown syntax to display a table. A recommended site would be 'https://www.tablesgenerator.com/markdown_tables'.

### Images
---------------------

  Images in lab reports are almost always a necessity. In most cases, when creating a lab report, the images will be hosted locally, though in some cases, images may be hosted on a website that is being referenced.

For images hosted on a website, the image address can be referenced directly.
- For example,`![Image](https://www.publicdomainpictures.net/pictures/370000/t2/kunstliche-intelligenz-1603866343eG3.jpg "random image")` generates <br>

![Image](https://www.publicdomainpictures.net/pictures/370000/t2/kunstliche-intelligenz-1603866343eG3.jpg "random image")

For images that are located on the local computer, the image can be added by using it's relative path.
- For example, `![Image2](/imgs/cover.jpg "cover image")` generates <br>

![Image2](./imgs/cover.jpg "cover image")

### Equations
---------------------

  Unfortunately, Markdown does not have a direct method for adding equations or mathematics symbols. Markdown does, however, offer direct HTML support which does allow for adding math symbols. It is worth noting that in formal documentation that is intended to be published, this formatting is less likely to be widely accepted. For a more professional display of equations, LaTex is recommended.

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

  A comprehensive list of HTML supported symbols can be found here, https://www.toptal.com/designers/htmlarrows/math/. "HTML ENTITY" is the syntax version that will be used  when creating an equation in Markdown.

## Conclusion

  Markdown and VSCode can be used to quickly create technical documentation. To demonstrate this is the case, this document has been created as a Markdown file. Students are encouraged to view the raw version of the document to see additional examples of the Markdown commands covered in this document. The raw Markdown file can be downloaded and referenced later as a cheat sheet.

## Links

VSCode Installation Files - https://code.visualstudio.com/download <br>
Table Generator - https://www.tablesgenerator.com/markdown_tables <br>
HTML Math Symbols - https://www.toptal.com/designers/htmlarrows/math/ <br>


| Input | Output |
|- |- |
|`*Italicizing this is easy!*` | *Italicizing this is easy!* |
|`**Bolding this is just as easy!**` | **Bolding this is just as easy!** |
| `***Bold and Italicized for the win!***` | ***Bold and Italicized for the win!*** |
