# Why is Markdown difficult in translation?

Because Markdown syntax uses symbols that can appear normally in a text and there are different symbols that have the same functionality, it is difficult for CAT software developers to create Markdown filters. The filters need to sift out the Markdown tags and place non-editable tags in a CAT program. The tags in the CAT must be non-editable to avoid an accidental editing or deletion.

However, some Markdown tags must be editable to certain degree:
```
[**Bold**](#bold)
![Shark](resources/images/IMG_20200401_210429.jpg "A Technical Writer Shark")
```
In the examples above, 