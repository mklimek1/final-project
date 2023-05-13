# Trados Studio 2022 — Results

## Default Settings
- unlike WF, it did analyse the whole table with formatting <!--- this should be in the comparison section !-->
- no errors with opening the default test file
- reads hover text
- interprets superscript as superscript
- does not interpret subscript as subscript
- ignoring markdown formatting is tricky
- majority of Markdown tags is converted not as tags, but as real bold, italics etc., which makes translation more difficult
- linking doesn't work
- inline code, code block don't work
- hover text got messed up
- content of HTML part got ignored lol
- the inline quote tag doesn't turn off HTML in one place, but it did in another, like `<p></p>`
![[Pasted image 20230506221617.png]]
- definition doesn't work (because it's in HTML tags)
- in `Unroll another section`, Markdown formatting is ignored, but not in the table
- 	- `<!--- comment --->` is ignored

## Handle line breaks as inline tags

Nothing changed

## Translate code blocks — Embedded Content Plain Text v 1.0.0.0

Code block indeed can be translated, but not inline.
Then, Markdown tags are plain symbols, e.g. asterisk remains an asterisk.

Still problems with hover text.
Still content of html is not translatable.

## Translate code blocks — Embedded Content SpreadsheetML v. 1

![[Pasted image 20230506225339.png]]

This is caused by backtick {\`}

## Translate code blocks — Html Embedded Content 5 2.0.0.0

![[Pasted image 20230506230602.png]]

For some reason, JavaScript code block gives that. Had to remove it, so it could be opened.

It differs in segmentation, but the general content stays the same.
Hover text wrong, g-dammit!

Locked `<code>tags</code>`

## Translate HTML blocks — Embedded Content Plain Text v 1.0.0.0

It is used in combination with Translate code blocks — Embedded Content Plain Text v 1.0.0.0, because it gave the least errors.

BIG THING - `<!-- -->` comment is editable!, but not `<!-- omit in toc -->`
Hover text wrong, g-dammit!

HTML tags appear as normal signs
Finally, content of `<html></html>` can be edited.

## Translate HTML blocks — Embedded Content SpreadsheetML v. 1

![[Pasted image 20230508173616.png]]
This is caused by `<` symbol.

## Translate HTML blocks — Html Embedded Content 5 2.0.0.0

`<!-- -->` comment is not editable!, but not `<!-- omit in toc -->`