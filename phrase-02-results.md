# Results

# Settings — Plain

Settings:
- Hard line break creates new segment 
- Import code blocks

Comments cannot be translated
Inline code can be translated, but pay attention to special characters
Strikethrough is not interpreted as tags
There's so much code/tags left, that it really requires attention to avoid editing something by accident.
E.g. emoji, HTML tags are left - risk in MT.
Reference is not translated, but hover text is
Some problems with interpreting `*` as italics, because the escape sign `\` was inserted
Ordered list was not interpreted correctly because the escape sign `\` was inserted
Unordered list was not interpreted correctly - it's as if `ENTER` was removed
Code block was not interpreted correctly because the escape sign `\` was inserted
Table was not interpreted correctly and in the output is just a collection of symbols
For some reason `**This _sums_ ~~~down~~~ ^up^:**` wasn't interpreted at all.
Footnotes were not interpreted correctly because the escape sign `\` was inserted
HTML block: the content is editable, but the tags are ignored as they should be
But  not the code block :)

# Settings — PHP/Python Markdown Extra

Settings:
- Hard line break creates new segment 
- Import code blocks

Comments cannot be translated
Inline code can be translated, but pay attention to special characters
Reference is not translated, but hover text is
Some problems with interpreting `*` as italics, because the escape sign `\` was inserted
Ordered list was not interpreted correctly because the escape sign `\` was inserted
Unordered list was not interpreted correctly - it's as if `ENTER` was removed
Code block interpreted correctly and editable
Comment in JS can be translated
Table works well
For some reason `**This _sums_ ~~~down~~~ ^up^:**` wasn't interpreted at all.
HTML block is editable, but it pastes all the tags alongside, so they need to be manually copied

# Settings — GitHub Flavored Markdown

Settings:
- Hard line break creates new segment 
- Import code blocks

Comments cannot be translated
Inline code can be translated, but pay attention to special characters
Reference is not translated, but hover text is
Lists work as intended
Code block interpreted correctly and editable
Comment in JS can be translated
Table works well
HTML block is editable, but it pastes all the tags alongside, so they need to be manually copied

This works best, so it will be used for other settings.

# Settings — Preserve whitespaces

Generally, the output is similar as in the Case of [Above](#Settings-github-flavored-markdown).

# Settings — Process YAML header

Is not covered - the test file doesn't include a YAML header.

# Settings — Exclude code elements

Excludes inline code, but code block remains.

# Settings — Exclude code elements with unchecked import code blocks

Excludes inline code and code block.