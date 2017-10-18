# Writing "MD" files that can be converted to HTML with MDreader

## 1. Basic MD Text Entry

Text is entered normally with only a single proportional font. Paragraphs must be separated by one (or more) lines of white space. Paragraphs are rendered with one line of white space between them even if two or more spacing lines are used in the text file. If no whitespace separates paragraphs MDreader will render them as one single continuous paragraph.

€¥$¢√π÷ etc. are handled correctly.
 
Extra spacing between paragraphs cannot be achieved easily.

All formatting codes (*, #, > etc.) must be followed by a space to work correctly in git.

There seems to be a problem with editing the README.MD text directly on Github via android and Firefox. Text changed and disappeared quite unpredictably. I did manage to make some changes to this file but odd word duplications occurred so I plan to upload a revision created offline (this version) and of README.md.

## 2. Bold & Italic Text

*Text enclosed by 1 asterisk (touching the text at each end)* - italic

**Enclosed by 2 asterisks (touching the text at each end)** - bold

***Enclosed by 3 asterisks (touching the text at each end)*** - italic + bold

One can use underline characters instead of asterisks.

****Enclosed by 4 asterisks (touching the text at each end)**** - no effect in QuickEdit but is interpreted as bold + italic in MdReader. This is followed by 3 lines of whitespace.



## 3. Indenting, Bullet point lists & Numbered lists.

>### Indenting

To achieve Indenting use one or more Chevrons (>) at the start of the paragraph. This can also be used in conjunction with Headings, Bulleted lists and Numbered lists

> Indented text following a right Chevron (>) &  space

>> And double indented following 2 right Chevrons (> >)

The Chevron(s) must be at the very start of the line.

> ### Bullets

* Text preceded by an asterisk and then a space - creates a bullet point.

* Another asterisk and Space

* A final asterisk and space

> * An indented bullet

>> * And now a double indented bullet (2 Chevrons and an asterisk)

>>> * And now a triple indented bullet (3 Chevrons and an asterisk)

>### Numbered lists

A numbered list item is formatted by starting a paragraph with any digit - e.g. 4. in the following list. The numbering is automatic (single digit). Just start each item with a digit, a dot and a space.

4. Starting a list with a 4. allows you to select the value of the first list item with a 4 in Github, but in QuickEdit and MDreader lists always start at 1.

1. Lots more information. Lots more information. Lots more information. Lots more information. Lots more information. Lots more information.

1. Extra item added into the list after the first 4 were created.

3. List item 3 with more text

5. List item 4

> 1. A Numbered list item with increased indenting. Note that when the indenting changes the numbering resets to 1. Numbering cannot be started at any number other than 1.

> 1. Some more text after 1 Chevron and a digit plus dot. There is **NO** automatic numbering of indented lists in Github this should be shown as item 2.



## 4. Variable Headings: each throws a single (standard) line space after it. The heading will word wrap.

###### Preceeded by Six hashes and a space
##### Preceeded by Five hashes and a space
#### Preceeded by Four hashes and a space
No \#s used on this line **4 \#s Appear equivalent to standard bold text (this).** 
###Preceeded by Three hashes and a space
##  Preceeded by Two hashes and a space
#  Preceeded by One hash and a space

## 5. Page width lines.
***
\*\*\* on a new line creates a pagewide line. Useful as a separator given that paragraph separation is not variable.
***


## 6. In Line Text

In line text is **not** supported by MDreader's html renderer, but is OK in QuickEdit. The character used (`) is found via the ?123 and then =\\< alternative keyboard. This is known as a'tickback' on github, it seems.

``` python

Code line 1
Code line 2 followed by whitespace

Code Line 3 followed by 2 lines of **whitespace** (this is shown bold by MDreader)


Code Line 4
Code Line 5

Code Line 6

```

Quoting code

You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted.

Use `git status` to list all new or modified files that haven't yet been committed.

Rendered inline code block

To format code or text into its own distinct block, use triple backticks.

Some basic Git commands are:
```
git status
git add
git commit
```



## 7. HyperLINKs

To create a clickable link to http://github.com/login - enter \[Git-Hub](http://github.com/login) Which appears thus: [Git-Hub](http://github.com/login)


## 8. Images
To insert an image into a document use: 
\!\[AnImage]\(/storage/emulated/0/documents/tmp/statusboard-statuszero-docs-master/images/status-zero.jpg) displays an image (see below).

![AnImage](/storage/emulated/0/documents/tmp/statusboard-statuszero-docs-master/images/status-zero.jpg)


## 9. Tables
Not supported by QuickEdit or the MdReader App, but are (supposed) to be supported on Github.

First Header|Second Header
------------|-------------
Content cell 1 | Content cell 2
Content column 1 | Content column 2


## 10. Conclusion
MarkDown is not standardised - it is different on Github, QuickEdit and MdReader. Using these methods in QuickEdit and MDreader will allow reasonably consistent results to be achieved.

