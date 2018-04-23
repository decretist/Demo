## DH Colloquium  
### Better Tools for Tracking Your Revisions: Pandoc and Markdown  
#### 7 March 2018

Based on the tutorial [Sustainable Authorship in Plain Text using Pandoc and Markdown](https://programminghistorian.org/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown) by Dennis Tenen and Grant Wythoff from [The Programming Historian](https://programminghistorian.org/)

### Motivation

### Zotero
* Highlight collection  
* Control-click on collection  
* Export collection as _project.bib_  
* You can hand-edit _project.bib_,
but you don't have to

### CSL
* Download CSL (Citation Style Language) style from the [Zotero Style Repository](http://www.zotero.org/styles/chicago-fullnote-bibliography)

### Pandoc and Markdown
* Generate reference doc:
```
pandoc --print-default-data-file reference.docx > myref.docx
```
* Edit main.md, then generate MS Word doc:
```
pandoc -o main.docx --filter pandoc-citeproc --reference-doc=myref.docx main.md
```
