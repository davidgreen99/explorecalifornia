# A better markdown cheatsheet

Based on "A better markdown cheatsheet" by Jon Schlinkert ( <https://gist.github.com/jonschlinkert/5854601> )

Cleaned up to satisfy Citrix GFM rules in markdownlint.

## Dashes

The following special characters are handy:

``` markdown
— M-dash (separator, in place of parentheses)    ALT + 0151
– N-dash (joins, for number ranges)              ALT + 0150
… ellipsis                                       ALT + 0133

```

## New section added in branch Tom

Double click on HelloWorld, and bring up our window that shows our uncommitted changes. Notice that our changes are unstaged, and so we're going to look at them. Program.cs has changed, here are the three lines that have been removed, and the two lines that have been added. And of course Runner.cs will be all added. We're going to click here to take all of our unstaged files and stage them. And now that they're staged, or in the index, we can commit them.

Renders to:

—  M-dash (separates, parenthetical )

–  N-dash (joins, use for number ranges)

… ellipsis

More special characters [here](https://www.keynotesupport.com/websites/special-characters-symbols.shtml).

## Headings

Headings from `h1` through `h6` are constructed by using a `#` for each level. ("MD003": Use # to denote headings.)

("MD024": Duplicate headings allowed in a file.)

("MD026": Do not use . , ; : ! "  } as the last character in a header (but ? is allowed at the end of a heading).)

``` markdown
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
```

Renders to:

# h1 Heading

## h2 Heading

### h3 Heading

#### h4 Heading

##### h5 Heading

###### h6 Heading

## Raw HTML

"MD033": Use only pure markdown. Raw HTML is not allowed.

## Horizontal Rules

In markdown, you can create HTML `<hr>` with 3 consecutive underscores (`___`), which renders to:

___

## Body Copy

"MD013":  Line length is not limited to 80 characters.

"MD009": Use 2 trailing spaces at the end of a line to denote a line break.

## Emphasis

### Bold

For emphasizing a snippet of text with a heavier font-weight.

The following snippet of text

``` markdown
**rendered as bold text**
```

renders to:

**Rendered as bold text**

### Italics

For emphasizing a snippet of text in italic face. The following snippet of text is _rendered as italicized text_.

``` markdown
_rendered as italicized text_
```

renders to:

_rendered as italicized text_

### Strikethrough

In GFM strike through text by enclosing in two tildes.

``` markdown
~~Strike through this text.~~
```

Which renders to:

~~Strike through this text.~~

## Blockquotes

For quoting blocks of content from another source within your document.

Add `>` before any text you want to quote.

``` markdown
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat an ante.
```

Renders to:

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat an ante.

Blockquotes can be nested:

``` markdown
> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>>> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
```

Renders to:

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor odio non est accumsan facilities. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>>> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.

## Alerts

Use blockquotes:

```
> Important:
>
> colon suffix, first line title use sentence case. The CSS automatically makes the first line bold and blue. Leaving the asterisks in place has no known side effects, although Beth stated in Slack "*the issue with leaving the asterisks is with potential fuzzy matches with Loc. I wouldn’t make a special effort to remove, just do as you can*."
>
> blank lines also start with chevron
```

renders as:

> **Important:**
>
> colon suffix, first line title uses sentence case. The CSS automatically makes the first line bold and blue. Leaving the asterisks in place has no known side effects, although Beth stated in Slack "*the issue with leaving the asterisks is with potential fuzzy matches with Loc. I wouldn’t make a special effort to remove, just do as you can*."
>
> blank lines also start with chevron

## Clickthroughs

Not this: “select **File**, select **New**, then select **Email**”

Use this: "select **File > New > Email**”

-  bold around everything
-  spaces around chevrons

## Lists

### Unordered

A list of items in which the order of the items does not explicitly matter.

Use either plus (**+**) or dash (**-**) symbols to denote bullets for each list item:

**Note**: *the first bullet symbol on the page* sets the valid symbol for the page!

"MD007": Use 4 spaces to indent nested lists. 4 spaces for each level of indent/nesting.

"MD030": Use 2 spaces between the list marker and the first character of the line

```markdown
-  dash (2 spaces after listmarkers)
    -  dash (4 spaces before indented items)
    -  "MD007": Use 4 spaces to indent nested lists. 4 spaces for each level of indent/nesting.

+  plus (2 spaces after listmarkers)
    +  plus (4 spaces before indented items)
    +  "MD007": Use 4 spaces to indent nested lists. 4 spaces for each level of indent/nesting.

```

For example

``` markdown
-  Lorem ipsum dolor sit amet
-  Consectetur adipiscing elit
-  Integer molestie lorem at massa
-  Facilisis in pretium nisl aliquet
-  Nulla volutpat aliquam velit
    -  Phasellus iaculis neque
    -  Purus sodales ultricies
    -  Vestibulum laoreet porttitor sem
    -  Ac tristique libero volutpat at
-  Faucibus porta lacus fringilla vel
-  Aenean sit amet erat nunc
-  Eget porttitor lorem
```

Renders to:

-  Lorem ipsum dolor sit amet
-  Consectetur adipiscing elit
-  Integer molestie lorem at massa
-  Facilisis in pretium nisl aliquet
-  Nulla volutpat aliquam velit
    -  Phasellus iaculis neque
    -  Purus sodales ultricies
    -  Vestibulum laoreet porttitor sem
    -  Ac tristique libero volutpat at
-  Faucibus porta lacus fringilla vel
-  Aenean sit amet erat nunc
-  Eget porttitor lorem

### Ordered

A list of items in which the order of items matters.

2 spaces after listmarkers.

Use `1.` for each number, numbering is applied automatically.

``` markdown
1.  Lorem ipsum dolor sit amet
1.  Consectetur adipiscing elit
1.  Integer molestie lorem at massa
1.  Facilisis in pretium nisl aliquet
1.  Nulla volutpat aliquam velit
1.  Faucibus porta lacus fringilla vel
1.  Aenean sit amet erat nunc
1.  Eget porttitor lorem
```

Renders to:

1.  Lorem ipsum dolor sit amet
1.  Consectetur adipiscing elit
1.  Integer molestie lorem at massa
1.  Facilisis in pretium nisl aliquet
1.  Nulla volutpat aliquam velit
1.  Faucibus porta lacus fringilla vel
1.  Aenean sit amet erat nunc
1.  Eget porttitor lorem

## Procedures with indented images

-  4 spaces (or a Tab) *before* images to get them to indent and numbering to continue
-  Blank line above image

``` markdown
1.  Lorem ipsum dolor sit amet
1.  Consectetur adipiscing elit

    ![Minion](http://octodex.github.com/images/minion.png)
1.  Integer molestie lorem at massa
1.  Facilisis in pretium nisl aliquet
1.  Nulla volutpat aliquam velit
1.  Faucibus porta lacus fringilla vel
1.  Aenean sit amet erat nunc
1.  Eget porttitor lorem
```

Renders to:

1.  Lorem ipsum dolor sit amet
1.  Consectetur adipiscing elit

    ![Minion](http://octodex.github.com/images/minion.png)
1.  Integer molestie lorem at massa
1.  Facilisis in pretium nisl aliquet
1.  Nulla volutpat aliquam velit
1.  Faucibus porta lacus fringilla vel
1.  Aenean sit amet erat nunc
1.  Eget porttitor lorem

## Code

### Inline code

Wrap inline code snippets with `` ` ``.

No spaces inside code snippets.

For example, `<section></section>` should be wrapped as "inline".

```html
For example, `<section></section>` should be wrapped as "inline".
```

### Indented code

You can indent several lines of code by adding at least 4 spaces:

```
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
```
renders as:

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code

### Fenced code blocks

-  Use 3 backticks ```` ``` ```` on a separate lines before and after to 'fence-in' multiple lines of code.
-  specify code format after first backtips (no space) to apply auto *syntax highlighting*.
-  In Citrix docs, renders inside a dark box with copy feature.

<pre>
```
Sample text here...
```
</pre>

 renders as:

```
Sample <strong>bold<\strong> text here...
```

#### Syntax highlighting

"MD040": is optional to specify a language for fenced code blocks.

GFM (GitHub Flavored Markdown) supports syntax highlighting. To activate it, simply add the file extension of the language you want to use directly after the first code 'fence', ` ``` `, and syntax highlighting is automatically applied in the rendered HTML. For example, to apply syntax highlighting to JavaScript code:

<pre>

```javascript
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```
</pre>

Renders to:

```javascript
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```

XML code:

```xml
<div class="highlight"><pre><span class="nx">grunt</span><span class="p">.</span><span class="nx">initConfig</span><span class="p">({</span>
  <span class="nx">assemble</span><span class="o">:</span> <span class="p">{</span>
    <span class="nx">options</span><span class="o">:</span> <span class="p">{</span>
      <span class="nx">assets</span><span class="o">:</span> <span class="s1">'docs/assets'</span><span class="p">,</span>
      <span class="nx">data</span><span class="o">:</span> <span class="s1">'src/data/*.{json,yml}'</span><span class="p">,</span>
      <span class="nx">helpers</span><span class="o">:</span> <span class="s1">'src/custom-helpers.js'</span><span class="p">,</span>
      <span class="nx">partials</span><span class="o">:</span> <span class="p">[</span><span class="s1">'src/partials/**/*.{hbs,md}'</span><span class="p">]</span>
    <span class="p">},</span>
    <span class="nx">pages</span><span class="o">:</span> <span class="p">{</span>
      <span class="nx">options</span><span class="o">:</span> <span class="p">{</span>
        <span class="nx">layout</span><span class="o">:</span> <span class="s1">'default.hbs'</span>
      <span class="p">},</span>
      <span class="nx">files</span><span class="o">:</span> <span class="p">{</span>
        <span class="s1">'./'</span><span class="o">:</span> <span class="p">[</span><span class="s1">'src/templates/pages/index.hbs'</span><span class="p">]</span>
      <span class="p">}</span>
    <span class="p">}</span>
  <span class="p">}</span>
<span class="p">};</span>
</pre></div>
```

## Tables

Markdown doesn't support:

-  table cells with more than one paragraph
-  spanned rows
-  spanned columns
-  any element (such as an image) in a cell.

Use pipes `|` as cell dividers. (the pipes do not need to be vertically aligned.)

You **must** underline the header with a line of dashes `----` (with pipes).

``` markdown
| Option | Description |
| ------   | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine     | engine to be used for processing templates. Handlebars is the default. |
| ext         | extension to be used for dest files. |
```

Renders to:

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

### Right aligned text

Adding a `colon` on the right side of the dashes below any heading will right align text for that column.

``` markdown
| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

| Option | Description |
| ------:| -----------:|
| Data   | Path to data files to supply the data that will be passed into templates. |
| Engine | Engine to be used for processing templates. Handlebars is the default. |
| Ext    | Extension to be used for destination files. |

## Links

### Bare URL

A bare link is a URL cited as a reference for some information without any accompanying information about the linked page.  Enclose in angle brackets:

```
<https://www.citrix.com>
```

renders as

<https://www.citrix.com>

### Text link to URL, no tooltip

```
[Assemble](http://assemble.io)
```

Renders to this (hover over the link to see URL):

[Assemble](http://assemble.io)


### Text link to URL, tooltip

```
[Assemble](http://assemble.io "Tooltip text")
```

Renders to (hover over the link to display the tooltip):

[Assemble](http://assemble.io "Tooltip text")

### Unlinked URLs

For URLs that we don't intend to be live links, write an inline code by enclosing in single ticks (`):

```
`https://<customername>.xendesktop.net/Citrix/StoreWeb/`
```

renders as unlinked text:

`https://<customername>.xendesktop.net/Citrix/StoreWeb/`

Works in-line as well:

This is a URL enclosed in single ticks (\`) in a sentence `https://` here's another `https://adfs.mycompany.com/adfs/ls`.

### Link to a heading, same page

No need to place an anchor; they get generated automatically when the page is published. Simply use a link based on the heading title. All lowercase and spaces replaced by dashes. **Hyphens in headings remain unchanged**. For example, to link to this heading:

```markdown
# Restore a Workspace Environment Management command-line
```

use this syntax:

```markdown
[linked text](#restore-settings-from-a-workspace-environment-management-command-line)
```

### Cross reference link to any article in docs.citrix.com

**NB** - must be an absolute path starting from '/en-us'. e.g.  `/en-us/xenmobile/server/topic.html`

```
[link text](/en-us/xenapp-and-xendesktop/current-release/... /<filename>.html)
```

[link text](/en-us/xenapp-and-xendesktop/current-release/... /<filename>.html)

## Images

Images have a similar syntax to links but include a preceding exclamation point `!`.

```
![Alt text](http://octodex.github.com/images/minion.png "optional tooltip text")
```

![Alt text](http://octodex.github.com/images/minion.png "optional tooltip text")

or for **Citrix** repo media:

```
![Alt text](/en-us/xenmobile/server/media/manage-devices-columns.png "The Stormtroopocat")
```

![Alt text](/en-us/xenmobile/server/media/manage-devices-columns.png "The Stormtroopocat")

Converted files include image links in this form: 

/en-us/xenmobile/server/media/manage-devices-columns.png

That form is required, as it's needed for localization.

Images *must reside in the folder media inside your repo*. (Although it is technically feasible to link to images in other repos, when a PDF is created images will be missing unless they are in the same repo!)

### YouTube videos

For embedded **YouTube videos**, visit the YouTube site and get the video ID. The following sources the thumbnail image directly from YouTube and links to the actual video, so when the person clicks the image/thumbnail they are taken to the video:

Notes:

-  ALT TEXT appears at both ends (to keep markdownlint happy)
-  use **HTTPS** protocol

```markdown
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE-VIDEO-ID/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE-VIDEO-ID "IMAGE ALT TEXT HERE")
```

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/6rwY7Q0Ay84/0.jpg)](https://www.youtube.com/watch?v=6rwY7Q0Ay84 "IMAGE ALT TEXT HERE")

 
Like links, images also have a footnote style syntax

``` markdown
![Alt text][id]
```

![Alt text][id]

With a reference later in the document defining the URL location:

[id]: http://octodex.github.com/images/dojocat.jpg  "The Dojocat"

    [id]: http://octodex.github.com/images/dojocat.jpg  "The Dojocat"