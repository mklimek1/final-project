# Summary

In general, Wordfast Pro 8 is a good tool to translate Markdown files despite the import error in the beginning.

## Advantages

- Markdown reference in links can be translated, which makes it possible to translate a table of content and all other references to headers in Markdown files
- Many filter settings allow rich configuration options for importing Markdown files
- Imports the content of embedded HTML code

## Disadvantages

- Inline code is ignored and cannot be translated
- Code block is ignored and cannot be translated
- Code comments are ignored and cannot be translated
- Bizarre behaviour of tables
- Very complex combinations of Markdown tags or with HTML tags may cause problems or make the Markdown tags rendered normally; however, in the case of HTML tags this has more to do with the general behaviour between HTML and Markdown tags

# Recommendations for translation of Markdown files in Wordfast Pro

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

## Recommendations for technical writers

- Avoid combining bold, italic, and strikethrough — some combinations may cause importing errors
- Instruct the translator about basic Markdown formatting, because some tags can be rendered normally
	- If references are translated, instruct the translator how to translate references and in what format: one hash symbol, no space between the hash symbol and the first word, small letters, and minus symbol instead of spaces; e.g. the reference to this section should be `#recommendations-for-technical writers`
- If inline code or code block are used and if they must be translated, instruct the translator about:
	- How to open a Markdown file
	- The syntax of inline code or code block
	- What is to be translated and what must not be edited
- If extended Markdown syntax or HTML tags, instruct the translator that there may be  characters that are not used in a standard way in the source language and tell the translator what to do with them
- Encourage the translator to report any characters that are not used in a standard way in the source language

## Recommendations for translators

- Tick all settings for best performance, even if it means pasting links
- Contact the technical writer if characters are not used in a standard way in the source language
- Take care not to edit something that may be a tag
- Carefully check the output file if something is not missing, especially in tables

---

Go to sections:
- [*Trados Studio 2022 — overview*](trados-00-overview.md)
- [*Phrase — overview*](phrase-00-overview.md)
- [*Overview*](top-comparison.md)

---
[Back to top](#summary)


