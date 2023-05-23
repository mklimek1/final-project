Phrase
===

# Summary

In general, Phrase is a good tool to translate Markdown files when specific settings are applied.

## Advantages

- Rich settings
	- Can be configured with regex and other rules
- Inline code can be translated
- Code block can be translated
- Imports the content of embedded HTML code

## Disadvantages

- Only GitHub flavoured Markdown yields satisfactory results
	- [Plain](phrase-02-results.md#settings-Plain) Markdown flavour creates an output file that is useless, as restoring it to a usable state would take much time
- Markdown reference in links cannot be translated, which makes it impossible to translate a table of contents or all other references to headers in Markdown files
- Many different features stop working in the output file, even though they look good in the editor
	- Notable exception: [GitHub flavoured Markdown](phrase-02-results.md#github-flavored-markdown)
- Comments `<!-- -->` are ignored and cannot be translated
- Emoji is rendered normally, which makes it difficult for Machine Translation

# Recommendations for translation of Markdown files in Phrase

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

## Recommendations for technical writers

- Inform the translator about basic Markdown syntax, because some tags can be rendered normally
- Inform the translator about HTML or quoted code syntax, because the content in the code block is rendered normally
- Instruct the translator to use [PHP/Python Markdown Extra](phrase-02-results.md#php**&#47;**python-markdown-extra) or [GitHub Flavoured Markdown](phrase-02-results.md#GitHub-flavored-markdown) and inform about their limitations
- Instruct the translator **NOT TO USE** [Plain Markdown flavour](phrase-02-results.md#settings-Plain) 
- If `<!-- -->` comments are to be translated, instruct the translator about:
	- How to open the Markdown file
	- The syntax
	- What is to be translated and what must not be edited
	- Alternatively, break the syntax, so the comment is imported into the CAT, and fix it yourself in the output file
- Inform the translator that the output file may look different from the source file
- Encourage the translator to report any characters that are not used in a standard way in the source language

## Recommendations for translators

- Use [PHP/Python Markdown Extra](phrase-02-results.md#php**&#47;**python-markdown-extra) if no lists are used, but footnotes are
- Use [GitHub Flavoured Markdown](phrase-02-results.md#GitHub-flavored-markdown) if lists are used, but not footnotes
- **DO NOT USE** [Plain Markdown flavour](phrase-02-results.md#settings-Plain) unless the source file consists of bold and italics only
	- for safety, do not use it at all
- Adapt the settings to your needs — if the inline code or code block do not contain translatable content, uncheck `Include code blocks` and `Exclude code elements` to avoid accidental editing
- Make sure you do not edit something that may be a tag when you translate the content of the inline code or code block
- Contact the technical writer if characters are not used in a standard way in the source language
- Make sure you do not edit something that may be a Markdown tag
- Make sure you do not edit an emoji, e.g., `:exploding_head:`
- Carefully check the output file for any missing elements

---

Go to sections:
- [*Trados — overview*](trados-00-overview.md)
- [*Wordfast Pro 8 — overview*](wordfast-00-overview.md)
- [*Comparison of CATs*](top-comparison.md)

---
[Back to top](#summary)
