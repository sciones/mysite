title: "Coding: Markdown Tutorial"
categories:
  - Coding
tags:
  - Coding
  - Markdown
---

Markdown is a lightweight markup language that allows you to write formatted text using a plain text editor. It is widely used for documentation, web pages, and online communication because it is simple and easy to read. Here's a tutorial on how to use Markdown:

### Headings
To create headings, use the `#` symbol. The number of `#` symbols you use determines the level of the heading. For example:

        # Heading 1
        ## Heading 2
        ### Heading 3

### Text Formatting
Markdown allows you to format text in a few ways:

Bold: Use `**` or `__` to make text bold. For example: 

        **This is bold text**

Italic: Use `*` or `_` to make text italic. For example: 

        *This is italic text*

Strikethrough: Use `~~` to create strikethrough text. For example:

        ~~This is strikethrough text~~

### Lists
Markdown supports both ordered and unordered lists. To create an unordered list, use `*` or `-`. To create an ordered list, use numbers followed by a period (`1.`). For example:

        * Item 1
        * Item 2
        * Item 3

        1. Item 1
        2. Item 2
        3. Item 3

### Links
To create a link, use `[text](URL)`. For example:

        [Google](https://www.google.com)

### Images
To insert an image, use `![alt text](image URL)`. For example: 

        ![Cat picture](https://placekitten.com/200/300)

### Code
To format code, use backticks (`` ` ``). For example: 

        `print("Hello world!")`

### Blockquotes
To create a blockquote, use `>`. For example:

        > This is a blockquote
        > It can span multiple lines

### Horizontal Lines
To create a horizontal line, use three or more dashes (`---`).

### Tables
To create a table, use `|` to separate columns and hyphens (`-`) to separate the header row from the content. For example:

        | Column 1 | Column 2 | Column 3 |
        | -------- | -------- | -------- |
        | Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
        | Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |

### Task Lists
To create a task list, use `- [ ]` for incomplete tasks and `- [x]` for complete tasks. For example:
        - [x] Complete task 1
        - [ ] Incomplete task 2

## Emoji
To add an emoji to your Markdown text, use the colon (`:`) followed by the emoji name and another colon (`:`). For example: 

        :smile: will render as 😀

## Code Blocks
To create a code block, indent each line of code by four spaces or one tab. Alternatively, you can use three backticks to create a fenced code block. For example:

        def hello_world():
            print("Hello, world!")

or

        ```python
        def hello_world():
            print("Hello, world!")


### Footnotes
To create a footnote, use `[^footnote]` where you want the footnote marker to appear, and then add the footnote text at the end of the document.``

### Abbreviations
To create an abbreviation, use the following syntax: `*[abbreviation]`: definition*. For example:

        The HTML specification defines the *[HTML]: HyperText Markup Language* language

### Definition Lists
To create a definition list, use `:` to separate the term from the definition. For example:

        Term 1
        : Definition 1

        Term 2
        : Definition 2a
        : Definition 2b

### Autolinks
To create an autolink, simply paste a URL in the text. For example: 

        https://www.google.com will automatically become a clickable link.

### Escaping Characters
To escape a character in Markdown, use a backslash (`\`) before the character. For example:

        \_ will render as _.

### Raw HTML
If you need to include HTML in your Markdown document, you can use raw HTML tags. For example:

        <div class="example">
        This is an example div.
        </div>

While Markdown is a relatively simple language, it can be used to create complex documents and web pages. With the features listed above, you should be able to format your text effectively and efficiently.