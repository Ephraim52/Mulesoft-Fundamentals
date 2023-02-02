# Mulesoft-Fundamentals

## Organization is Key
This repository shall be your knowledge base and portfolio. With all the exercises you will do and the results you will get it is easy to lose structure. Below is a an overview on how to structure your repository:
```
root
 |- 00_includes < A place for your screenshots
 |- 00_templates < A place you will find the templates
 |
 |- 01_Linux_1
 |
 |- 02_Cloud_1
 |- 02_Cloud_2
 |- 02_Cloud_⋮
 |- 02_Cloud_6
 |
 |- 03_Project
 |  |- Code
 |  |- Documentation
 |  |- Log
 |
 |- descriptions < To prevent duplicate (inconsistent) descriptions you can use this folder and then link to it from your exercises.
```
**It is vital that you use this folder structure for your exercises.** This will make it easier to find the exercises and the results and for your teammembers and learning coaches to check your content and provide feedback.

As you can see the folders for the first few weeks are already made for you. Some of them will have an `.exist`-file. You can delete this file when you start filling them with your content.

## Definition of Done
Pushing the documentation to the repository is not the end of the assignment. We use 'the Four eyes' principle: this means that there should be two extra sets of eyes that validate and sign off your work before we consider it done. You will find the instructions for this in the presentation shared with you by the Learning Coach.

## MarkDown Tips
**A complete cheatsheet can be found [here](https://devhints.io/markdown)**.

### What isn't mentioned on the cheatsheet,
But is important to know:
```
If·you·write·a·line·and·use·one·break.↩
Github/Markdown·will·render·it·as·a·single·line.
```
If you write a line and use one break.
Github/Markdown will render it as a single line.

Use two breaks to make a paragraph.
```
Paragraph·1↩
↩
Paragraph·2
```
To only have a line break use a double space before you start a new line.

```
Line·1··↩
Line·2
```
Line 1  
Line 2
### Formatting shortlist
`[text](link)` is used to create links. Make certain that when you do link to a screenshot or another file, that you use relative paths.

`#·text` will format to a level 1 heading `<h1>`.

`##·text` will format to a level 2 heading `<h2>`.

And so on.

```
Text in `backquotes` will be formatted as code.
```

`*text*` will format as *italic text*.  
`**text**` will format as **bold text**.  
`***text***` will be both ***italic and bold***.

Look at the source of this Readme!
Space for filing my assignments, etc.
