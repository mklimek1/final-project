General recommendations
===

# Overview

This section includes general recommendations for technical writers (or generally, authors writing in Markdown) and translators. The recommendations are not specific for any particular CAT, so they can be used with other CATs as well.

## Recommendations for technical writers

<!-- @Marta - to mój taki *freestyle* z tymi radami, co mi przyszło do głowy i wydawało się zdroworozsądkowe; zdaję sobie sprawę, że życie dokumentalistyczne by tu dopisało więcej porad-->

In these recommendations, it is assumed that the technical writer contacts a translator who has little knowledge about Markdown.

- Inform the translator about basic Markdown syntax, because some tags can be rendered normally
- As in writing in general, use simple Markdown formatting — do not combine all possible formatting just to make the text really stand out
- Brief the translator on the following issues:
	- What is the scope of translation?
	- Do comments, inline code, and code blocks need to be translated?
	- Does embedded HTML need to be translated?
	- What must or must not be translated with regard to syntax
	- How to open Markdown files to check the output file
	- What to do with missing translations because some parts were not filtered by a CAT, for instance:
		- instruct how to open a Markdown file and how to edit it safely (if the translator has some background knowledge in coding)
		- ask the translator to provide missing translation in a separate text file and enter it on your own in the Markdown output file (if the translator does not have background knowledge in coding; this solution is generally safer)
- Discourage the translator from using machine translation tools because they may translate parts of the code, emojis, and similar content that should not be translated
	- Even if the translator knows Markdown or generally coding, there is still the risk that something will be edited by the machine translation tool and this will not be detected in checks and other quality assurance steps
- Encourage the translator to report:
	- Any characters that are not used in a standard way in the source language
	- Any deviations in the output file from the source file
	- Any missing translations in the output file

## Recommendations for translators

In these recommendations, it is assumed that the translator has basic knowledge of Markdown.

- If not briefed by the technical writer, ask the following questions:
	- Do comments, inline code, and code blocks need to be translated?
	- Does embedded HTML need to be translated?
	- Is there anything out of ordinary in the Markdown files?
	- Is there anything that requires special care in the Markdown files?
- Choose Markdown filters in the CAT adequately to the source file and the technical writer's brief
- If you have several CATs, it may be advisable to use several of them to translate the whole content of the Markdown files
- Do not use machine translation tools because they may translate parts of the code, emojis, and similar content that should not be translated
	- If machine translation is required by the client or translation agency, pay special attention to code elements because they may have been accidentally edited
- If there are missing translations because the CAT could not import given sections, ask the technical writer:
	- if you are to open the Markdown files and translate the sections within them
	- if yes, what programs are recommended to open the Markdown files
	- if not, what is the preferred method of providing missing translations (e.g. text files?)
- Carefully check the output file for any missing elements, wrong formatting, etc.
- Immediately contact the technical writer in case of technical problems with the source or output file, or any doubts with the project

---

Go to section: [*Conclusion*](top-conclusion.md)

---

[Back to top](#Overview)