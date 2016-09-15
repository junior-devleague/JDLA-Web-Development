---
title: "Syntax and structure"
published: true
morea_id: reading-syntax-structure
morea_summary: "Understanding how to write HTML"
morea_type: reading
morea_sort_order: 9
morea_labels:
 - HTML
 - syntax
---

# Syntax and Structure

Before we can write any code in html, there are some things we have to go over. One of those things is basic syntax. 

## What is “syntax”?

Syntax is a set of rules that must be followed. Every language has its own syntax; for example, the English language requires that we end our sentences with a punctuation mark, begin with capital letters, use proper pronouns, etc. Computer languages have syntax too. **You can think of syntax as the grammar or sentence structure of a language.**

Right now, we’ll go over the basic syntax of HTML, which you’ll need for the rest of this module.

## Elements and tags

At its most basic level, all HTML is is a series of carefully nested elements. HTML documents are comprised of multiple elements to provide content and structure to a document or web page.

In HTML, with a few exceptions (which we will go over later), all elements/tags have an opening and closing _tag_. A tag looks like this:

```html
<tagname>Content goes here...</tagname>
```

An **opening** tag is declared when the tag name is enclosed by angle brackets (greater than and less than symbols).

```html
<tagname>
<!-- An example of an opening tag-->
```

A **closing** tag is declared when there is a forward slash `/` before the tag **name**.

```html
</tagname>
<!-- An example of a closing element tag-->
```

An HTML element is defined as everything from the opening tag to the closing tag:

```html
<p>My first paragraph.</p>
<!-- An example of a paragraph tag in HTML. The <p> </p> tags and what goes inside is considered a single element in HTML-->
```
We also have comments, denoted by `<!-- Comment here -->`, which are just little notes for the coder, and ignored by the computer/browser. 

## Creating your first web page

Now that you can write tags, we can move on to creating your first web page.
However, there are still a few more things we have to go through before we can view our webpage.

The first thing we must discuss is the HTML skeleton:

### The HTML Skeleton
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Example Web Page</title>
    </head>
    <body>

   </body>
</html>
```

Please type the code into your index.html file, **with the correct indentation!**

**Also, it’s important to write your closing tag immediately after writing your opening tag before any nested content.** This makes it easier to see what goes inside of what and to make sure you end elements properly. If you don’t do this, after some point you won’t be able to keep track of all the tags you’ve opened.

Now, we can go over what each part means. 

Let’s start with the first line:

```html
<!DOCTYPE html>
```

This is your DOCTYPE declaration, and _must be the first line in every HTML document_. This line tells the browser what type of document we are working with. 

```html
<html>

</html>
```

This tag is used indicate that everything within the opening and closing tags is HTML code. Any and all HTML needs to be inside of this element.

```html
<head>

</head>
```

The head tag is used to provide information about the webpage. **None of the code inside the head tag will be displayed on your web page.** You also link together your scripts, stylesheets, and more inside the head.

A tag you must have inside the head tag is the `<title></title>` tag. You see the contents of the `<title>` tag written on the tabs of your browser. 

You also need to provide metadata (descriptions of your website, defining the character set you’re using, etc.) to the browser in the head tag. 

```html
<body>

</body>
```

The body tag contains all the content that is seen and displayed on your website. 

## Congratulations

You now have a HTML file that you can edit!

Try typing some text in the body tag and then open the HTML file in your browser.

Drag the HTML file onto the browser icon on your Desktop. **The browser you will be using for this class is Google Chrome.**

---

[Click here](https://junior-devleague.github.io/JDLA-Web-Development/morea/3_Basic_HTML/reading-tags-elements.html) to move on to the third reading, “Tags and Elements”.
