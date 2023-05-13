# Wordfast — Results

How tags are shown
![[Pasted image 20230506130422.png]]

- It does not open the Test File:
![[Pasted image 20230505195326.png]]
- This part is the culprit
	- `- this **simply ~~*wrong*~~**`
	- `~~this is *__bold__ but folly*, so I crossed it out~~`

To be precise, using bold and italics next to each other within strikethrough (or outside) may cause problems. See the WF-error.md file.


In a table, bold and italics are interpreted as asterisks. But no worry - they're then interpreted as formatting tags.
Adding asterisks adds formatting — I guess it does for anything entered into it.

For some reason, only one cell in the table got imported into Wordfast Pro.

- WF doesn't support its own italics, bold, underline, superscript - you can't add them
	- but just use asterisks to create
- WF has difficulties with complicated Markdown Syntax 
- What doesn't work in interpretation in default settings:
	- subscript is ignored and rendered as normal symbols
	- superscript is ignored and rendered as normal symbols
	- footnote is ignored and rendered as normal symbols
	- formatting (even standard MD formatting) in unrolled section is ignored and rendered as normal symbols
	- ignores inline code `this is not translatable`

# Default format settings — Extract Table Headers

Reference in links cannot be translated — this makes Table of Contents useless and any other references inside the document.

Hover text in image cannot be translated.
The comments are not visible.
HTML `<code>text</code>` allows translating text!
- `[text]` in table is ignored
	- `![text]` is ignored
	- hover text is ignored
	- links in TOC get ignored - `[coś-tam](#something)` doesn't work at all!
	- `<!--- comment --->` is ignored
	- block code content is ignored

# Extract Image Alt Text

Like the name - image alt text is now translatable.

# Extract Image Link Value

Like the name — link values are extracted.

# Extract Image Title

Like the name - hover text possible.

# Extract Href Link URL Value

It's possible to edit internal links, so TOC works
For some reason, the missing content in the cells appeared...but not fully, so it's Jan, but not "The Fearless".

# Extract Href Link URL Title

Works as intended.

# Tables

`_`causes problems in tables
However, I've used in another column `**` and it doesn't work

```
| No. | Name | Surname | Photo | Age |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**John *the Fearless***](https://en.wikipedia.org/wiki/John_the_Fearless) | [**Valois**](https://en.wikipedia.org/wiki/House_of_Valois) | ![John the Fearless](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "John the Fearless")|   48 |
```

vs.

```
| Lp. | Imię | Nazwisko | Zdjęcie | Wiek |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**Jan *bez Trwogi***](https://en.wikipedia.org/wiki/John_the_Fearless) | [](https://en.wikipedia.org/wiki/House_of_Valois) | ![John the Fearless](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "John the Fearless")|   48 |
```

But, it's enough to use default format settings + Extract Href Link URL Value




