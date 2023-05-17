# Why is Markdown difficult for CATs?

Because Markdown syntax uses characters that can appear in a text in their normal use and there are different characters that serve the same purpose, it is difficult for CAT software developers to create good Markdown filters. The filters need to sift out Markdown tags and place non-editable tags in a CAT program. The tags in the CAT must be non-editable to avoid an accidental editing or deletion.

However, some Markdown tags must be editable to a certain degree:
```
1. [**Bold**](#bold)
2. ![Shark](resources/images/IMG_20200401_210429.jpg "A Technical Writer Shark")
```
In the first example, `**` is a tag for **bold**. We do not want the CAT to interpret it as two asterisks, because they may be accidentally changed or deleted. As a result, the CAT should place a non-editable opening tag where the text in bold starts and a closing tag where the text in bold ends.

In the second example, the whole line is a reference to a displayed image file with a hover text `A Technical Writer Shark`. In this case, we want the CAT to interpret `Shark` and `A Technical Writer Shark` as translatable, but leave the brackets and link to the image file as non-translatable.

The difficulty lies in using such filters that interpret asterisks or brackets as Markdown tags, while also interpret them as normal characters used in the text, like `The Markdown file extension is *.md ("md" stands for Markdown)`. This is made difficult even further when combined with other characters that build up Markdown tags.

Markdown filters in Phrase, Trados Studio 2022, and Wordfast Pro 8 were tested on various Markdown tags in different combinations. A special test file was created for this purpose.

---

Next section: [*The test file*](ref-test-file.md)

---

[Back to top](#why-is-markdown-difficult-in-translation&#63;)