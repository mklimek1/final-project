# Summary

In general, Trados Studio 2022 is a good tool to translate Markdown files. However, it shows strange behaviour and errors in some of the settings.

## Advantages

- Imports a lot of content in default settings, e.g.:
	- link descriptions
	- hover text
- Code block can be translated
- Comments `<!-- -->` can be translated
- Imports the content of embedded HTML code, but only in `Html Embedded Content 5 2.0.0.0`

## Disadvantages

- Bizarre behaviour of hover text between different references
- Markdown reference in links cannot be translated, which makes it impossible to translate a table of contents or all other references to headers in Markdown files
- Inline code is ignored and cannot be translated
- HTML in the `Embedded Content Plain Text v 1.0.0.0` filter is rendered normally

# Recommendations for translation of Markdown files in Trados Studio

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

## Recommendations for technical writers

- Inform the translator about basic Markdown syntax because tags in code block are rendered normally
- If references are to be translated, inform the translator about:
	- How to open a Markdown file
	- The syntax: one hash symbol, no space between the hash symbol and the first word, small letters, and minus symbol instead of spaces; e.g., the reference to this section should be `#recommendations-for-technical writers`
- Inform the translator about HTML or quoted code syntax, because the content in the code block is rendered normally
- If possible, use code block even for inline code because inline code cannot be translated
- Encourage the translator to report any characters that are not used in a standard way in the source language
- Be aware that some content between different HTML tags may or may not be imported into Trados and, as a result, translated

## Recommendations for translators

- Adapt the settings to your needs — if the embedded HTML does not contain content to be translated, untick the `Translate HTML block` box
	- This way you do not risk accidental editing of the HTML code
- Make sure you do not edit something that may be a tag when you translate the content of the code block
- Contact the technical writer if characters are not used in a standard way in the source language
- Be aware that some content between different HTML tags may or may not be imported into Trados and, as a result, translated
- Carefully check the output file for any missing elements or elements placed incorrectly, e.g., hover text


---

Go to sections:
- [*Phrase — overview*](phrase-00-overview.md)
- [*Wordfast Pro 8 — overview*](wordfast-00-overview.md)
- [*Comparison of CATs*](top-comparison.md)

---
[Back to top](#summary)
