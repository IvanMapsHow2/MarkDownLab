# Markdown: What is it?
Last Edited on 2024-07-24

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

### Ordered List
An ordered list (a list in which sequence is important) can be made by simply starting lines with 1, 2, 3...
1. Identify the flavor of Markdown supported by the platform.
2. Write Markdown in that flavor.
3. Convert Markdown to HTML.

### Unordered List
An unordered list (a list in which sequence isn't important) can be made by beginning lines with **-**.
- bananas
- peanut buter
- apple sauce
- tuna
- corn flakes

##### Code Block
Make a block of code look like a block of code by a hard return followed by lines that start with at least 4 spaces.

    def get_count(the_data_object):
        return arcpy.GetCount_management(the_data_object).getOutput(0)
        
##### Code Block - Another Way, Using Fenced Code Block
Another way to present a block of code is fence the code with ==```==
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

##### Hyperlink
Text that is a URL can be immediately made into a hyperlink.
>For more information, go to <https://vcgi.vermont.gov>.

Otherwise, text can be quickly hyperlinked with a ==[text to show] (URL)== pattern.
>[VCGI](https://vcgi.vermont.gov) is the Vermont Center for Geographic Information.

##### Image
An image is added with an ==![alternative text] (URL "Title")== pattern.
![tractor picture](http://maps.vcgi.vermont.gov/opendata/images/icons/data_themes/Agriculture-Icon.svg "tractor")

##### Table
Use a combination of ==- - -== and ==|== to make a table.
| Version           | Release Date     |
| ---               | ---              |
| 1.0               | 2012-04-30       |
| 1.1               | 2013-06-20       |
| 1.2               | 2015-07-08       |
| 2.0               | 2017-09-09       |

##### Footnote
A footnote is a hyperlinked superscript number that links to an anchor somewhere on the page. To make the superscipt part, use a ==[^footnote identifier]== pattern. To make the anchor, use a ==[^footnote identifier]: info== pattern. Regardless of the identifiers that are used, footnotes are number sequentially, starting with 1.
>Use the REST[^2] protocol.
>[^2]: Representational State Transfer protocol.

##### Definition List
A definition list can be quickly created by entering a term followed by lines that begin with ==:==. Notice that the terms can be made bold by using ==**== (Markdown syntax).

**Cadastre**
: An official register of locations, values, and other characteristics of real properties.

**Cadastral**
: Something that is a component of or is related to a cadastre.

##### Strikethrough
A horizontal line can be marked through text by using ==~~~==.
>Supported data formats include file geodatabase, ~~~shapefile~~~, and GeoPackage.

### Positives of Markdown
- It's easier to write than HTML (creating and filling XML tags).
- In raw form, it's easer to read than HTML.
- When its text is rendered in HTML, Markdown options can make the text content easier to read.
- It automatically escapes characters like ==<== (`&lt;`) and ==&== (`&amp;`).
- It is 

### Getting Help with Markdown
<https://www.markdownguide.org/> is a superb resource for learning Markdown and finding resources for using Markdown.








