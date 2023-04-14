---
title: "Coding: Getting Started with Jekyll"
date: 2023-04-11
categories:
  - Coding
tags:
  - Coding
  - Jekyll
toc: true
toc_label: "Jekyll"
toc_icon: "cog"
---

Jekyll is a static site generator that takes text written in your favorite markup language and uses layouts to create a static website. You can tweak the site's look and feel, URLs, the data displayed on the page, and more.

### Jekyll to build a website

Here are the steps on how to:

1. Install Jekyll. You can install Jekyll with the following command:

        gem install jekyll

2. Create a new Jekyll site. Once Jekyll is installed, you can create a new Jekyll site with the following command:

        jekyll new mysite

This will create a new directory called mysite with all the files you need to start building your website.

3. Add content to your website. You can add content to your website by creating Markdown files in the _posts directory. Each Markdown file will be converted into a separate page on your website.
For example, if you create a file called 2023-02-24-my-first-post.md, it will be converted into a page called /2023/02/24/my-first-post.

4. Create a layout for your website. A layout is a template that Jekyll uses to generate your website's pages. You can create a layout by creating a file called index.html in the _layouts directory.
The index.html file will contain the basic structure of your website's pages. You can then add additional content and styles to your pages by editing the index.html file.

5. Customize your website's look and feel. You can customize the look and feel of your website by editing the _sass and _css directories. The _sass directory contains Sass files, which are used to generate CSS files. The _css directory contains the CSS files that are used to style your website.
You can also use Jekyll's built-in variables to customize your website's look and feel. For example, you can use the site_name variable to set the name of your website.

Publish your website. Once you're happy with your website, you can publish it by running the following command:

        jekyll serve
        
This will start a local server that you can use to view your website. You can then share your website's URL with others.

Jekyll is a powerful tool that you can use to build beautiful, static websites. With a little bit of effort, you can create a website that looks and feels just like you want it to.

### How to Make a Markdown File for Jekyll

Here are the steps on how to make a markdown file for Jekyll:

1. Create a new markdown file.
You can create a new markdown file by opening a text editor and creating a new file with the extension .md.

2. Add markdown syntax to your file.
Markdown is a simple markup language that is easy to learn. You can use markdown to create headings, lists, tables, and more.

3. Save your file.
Once you have added markdown syntax to your file, save it.

4. Add your markdown file to your Jekyll site.
You can add your markdown file to your Jekyll site by placing it in the _posts directory.

5. Build your Jekyll site.
Once you have added your markdown file to your Jekyll site, you can build your site by running the following command:

        jekyll build

This will create a static website from your markdown files.

Here is an example of a markdown file:

        # This is a heading

        ## This is a subheading

        ### This is a sub-subheading

        This is some text.

        Here is a list:

        * Item 1
        * Item 2
        * Item 3

        Here is a table:

        | Column 1 | Column 2 |
        |---|---|
        | Item 1 | Value 1 |
        | Item 2 | Value 2 |
        | Item 3 | Value 3 |

This markdown file will be converted into the following HTML:

        <h1>This is a heading</h1>
        <h2>This is a subheading</h2>
        <h3>This is a sub-subheading</h3>
        This is some text.

        <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        </ul>

        <table>
        <thead>
        <tr><th>Column 1</th><th>Column 2</th></tr>
        </thead>
        <tbody>
        <tr><td>Item 1</td><td>Value 1</td></tr>
        <tr><td>Item 2</td><td>Value 2</td></tr>
        <tr><td>Item 3</td><td>Value 3</td></tr>
        </tbody>
        </table>

As you can see, markdown is a very simple and easy-to-use markup language. You can use it to create beautiful, static websites with Jekyll.