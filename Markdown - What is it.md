# Markdown: What is it?
Last Edited by Ivan Brown on 2024-07-24

## Markdown is Composed of 2 Things
- a language for creating web content using syntax in a text file that is much lighter than HTML tags
    (has an original basic syntax and several spin-off flavors)

- a tool that converts markdown to HTML
    (several tools are available)

Credit: [John Gruber](https://daringfireball.net/projects/markdown/)

## How Markdown Works--In General
1. Using markdown syntax (a particular flavor), write content in a text editor.

2. Use a tool that is compatible with markdown syntax to convert text to HTML.
    (Some tools can also convert markdown to PDF.)

Credit: [John Gruber](https://daringfireball.net/projects/markdown/)

## Markdown Conversion and Markdown Flavors
Markdown is converted to other formats (HTML) either by using a platform's supported-markdown functionality (e.g., GitHub repository `README.md` files, GitHub gists, `WordPress.com` sites, etc.) or by inputting markdown text into one of several markdown-conversion tools.

Each platform or conversion tool runs on a particular flavor of markdown. The [original flavor](https://daringfireball.net/projects/markdown/) was created by John Gruber in 2004. Now several other flavors exist--as superset derivatives.

[CommonMark](https://spec.commonmark.org/0.29/) is a specification that attempts to more clearly specify Markdown syntax. [GFM](https://github.github.com/gfm/) (GitHub Flavored Markdown)--a markdown flavor used in GitHub--is a superset of the CommonMark specification. Another CommonMark-superset flavor is Markdown used by the [Dillinger](https://dillinger.io) open-source web-based markdown editor. Dillinger runs on a converter called [markdown-it](https://github.com/markdown-it/markdown-it), which runs on a CommonMark superset (a couple of syntax extensions are from GFM).

## A Few Interesting Examples (using GFM)

### Code Span (short inline code) 
Highlight the code by beginning and ending text with **`**. 

Example: `print("Hello World!");`

### Fenced Code Block
Illustrate code by beginning and ending text with **```** 

Example...
```
def get_index(the_list, the_string):
   found_it = False
   i = 0
   while i < len(the_list) and found_it == False:
      if the_list[i].upper() == the_string.upper():
         found_it = True
      else:
         i += 1
   if found_it == True:
      return i
   else:
      return -1
```

### Header Levels
Begin a line w/ a `#` for a top-level header. Then, for sub-headers and sub-sub-headers and so on, increase the number of `#`, i.e., `###`.

### Bold (Emphasized Text)
Wrap the text to be bold with `**`.

Example: I want **this text** to be bold.

### Italics
Wrap the text to be in italics with `*`.

Example: I want *this text* to be in italics.

### Italics and Bold
Wrap the text to be in italics and bold with `***`.

Example: I want ***this text*** to be in italics and bold.

### Strikethrough
Wrap the text to be in strikethrough with `~~`.

Supported data formats include file geodatabase, ~~shapefile~~, and GeoPackage.

### Hard Return  
To force a hard return, end line of text with 2 or more spaces followed by return.

Example:  Here's a line of text followed by 2 spaces.  
And here's another line.

### Thematic Break Line 
`---` Makes a thematic break line.

Example: 

---

### Paragraphs 
Use a blank line to separate paragraphs.

Paragraph 1

Paragraph 2

### Ordered List
An ordered list (a list in which sequence is important) can be made by simply starting lines with 1, 2, 3...

Example...
1. Identify the flavor of Markdown supported by the platform.
2. Write Markdown in that flavor.
3. Convert Markdown to HTML.

### Unordered List
An unordered list (a list in which sequence isn't important) can be made by beginning lines with `-`.

Example...
- bananas
- peanut buter
- apple sauce
- tuna
- corn flakes

### Task List
Make a list of un-checked and/or checked tasks with the pattern `- [ ] Task Description` or `- [x] Task Description`.  

Example...  
- [x] Mow the lawn
- [ ] Clean the gutters

### Hyperlink
Text that is a URL can be immediately made into a hyperlink. 

Example: For more information, go to https://vcgi.vermont.gov.

Otherwise, text can be quickly hyperlinked with a `[text to show] (URL)` pattern. 

Example: [VCGI](https://vcgi.vermont.gov) is the Vermont Center for Geographic Information.

### Image
An image is added with an `![alternative text](URL "Title")` pattern. 

Example...  
![tractor picture](http://maps.vcgi.vermont.gov/opendata/images/icons/data_themes/Agriculture-Icon.svg "tractor")

### Table
Use a combination of `---` and `|` to make a table.  

Example... 
| Version           | Release Date     |
| ---               | ---              |
| 1.0               | 2012-04-30       |
| 1.1               | 2013-06-20       |
| 1.2               | 2015-07-08       |
| 2.0               | 2017-09-09       |

### Footnote
A footnote is a hyperlinked superscript number that links to an anchor somewhere on the page. To make the superscipt part, use a `[^footnote identifier]` pattern. To make the anchor, use a `[^footnote identifier]: info` pattern (it automatically renders at bottom of the page, even if it's located mid-page). Regardless of the identifiers that are used, footnotes are number sequentially, starting with 1.  

Example...  
Use the REST[^2] protocol.  
[^2]: Representational State Transfer protocol.

### Blockquotes
Add a `>` at the beginning of the paragraph.  

Example...
>In SQL Server–out-of-the-box, the **sp_spaceusedstored** procedure can be used to see the amount of disk space a particular table (layer) consumes.

For a multi-paragraph blockquote, add a `>` followed by a return between paragraphs to make blank lines. Example...  

>All geodatabases that exchange data via the **EGC Geospatial Data Exchange Protocol** must be in a geodatabase release that is supported by Esri for both **ArcGIS Desktop** and **ArcGIS Pro**-–this means that currently, data exchanged via the protocol must be in a geodatabase release of **10.3.1** or higher.
>
>Currently, hub geodatabases are in geodatabase release **10.5.1**. They are located in an instance of **Microsoft SQL Server 2016 (64-bit)**; a SQL Server client of **2012** or higher is required for connecting.

### Getting Help with Markdown
[A Guide on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).  









