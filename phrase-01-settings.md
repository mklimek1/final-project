Phrase
===

# Settings

The window with Markdown filters in Phrase looks like this:

![phrase-filter-settings](./resources/images/screenshots/Pasted-image-20230508233111.png)

*Figure 1: default Markdown filters in Phrase*

Phrase has the following filter settings for Markdown:
1. `Flavor` (only one can be selected):
	- `Plain`
	- `PHP/Python Markdown Extra`
	- `GitHub Flavored Markdown`
2. `Hard line break creates new segment` (default)
3. `Preserve whitespaces`
4. `Process YAML header` (not covered — the test file does not include a YAML header)
5. `Import code blocks` (default)
6. `Exclude code elements`
7. `Convert to Phrase TMS tags` (uses regex; requires a list of items)
8. `Custom elements (converted to Phrase TMS tags)` (requires a list of items)
9. `Non-translatable blocks` (requires a list of items)
10. `Don't escape characters` (requires a list of items)

The settings that require a list of items are not covered in this project. The reason is that there are many options and fringe cases that a user may want to configure. This is beyond the scope of the project. The project focuses only on the filters already configured in the software.

The default settings were used as the basic settings in the study. First, the Markdown flavours were checked. Then, further settings were added in the order from top to bottom.

The behaviour of the settings is described in the [Phrase — results](phrase-02-results.md) section.

---

Go to section: [*Phrase — results*](phrase-02-results.md)

---

[Back to top](#settings)