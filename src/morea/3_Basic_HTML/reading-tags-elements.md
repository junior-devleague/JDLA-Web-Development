---
title: "Tags and Elements"
published: true
morea_id: reading-tags-elements
morea_summary: "An explanation of HTML tags"
morea_type: reading
morea_sort_order: 10
morea_labels:
 - HTML
---

# Tags and Elements

All HTML code is comprised of a series of tags. In order to make a functional website, tags must be used very carefully, and it’s often not obvious why we use certain tags where we do. This is to organize your website’s content into easy-to-manage sections, as well as for styling and scripting purposes. 

Here we have our HTML skeleton:
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

You’ve already learned what types of data go into `<head>` and `<body>`. Every single HTML document must follow the structure above. 

One of the most common tags you will using is the `<p>` tag. The `<p>` tag defines a paragraph. In HTML, you need to indicate different paragraphs by using the `<p>` tag, because the browser registers everything that is not in a tag as plaintext, and it will ignore indents and extra spaces. 

In your index.html file, delete whatever you’ve written inside of the `<body>` tags before, and add the following: 

`<p>Hello World</p>`

From now on, do **NOT** enter any plaintext into your HTML code. Everything should be enclosed in a tag.

Your file should now look something like this:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>Example Web Page</title>
	</head>
	<body>
		<p> Hello World </p>
	</body>
</html>
```

Open this file in Google Chrome. 

Congratulations! You’ve just made your first (albeit, very basic) website! 

Please note the _indentation_. While spacing does not matter in HTML, it is important as a coder to indent elements that are within other elements. For example, the following: 

`<!DOCTYPE html><html><head><meta charset="utf-8"><title>Example Web Page</title></head> <body><p> Hello World </p></body></html>`
 
Is the exact same to the browser as what’s in your file right now. But that’s a lot harder to read, right? Browsers don’t care about how your code looks, but once your page gets filled with more and more elements, it’ll become extremely confusing. So, we need to indent the `<p>` element to indicate that it’s _inside_ the body of the page. 

Deciding what tags to nest inside of other tags is a huge part of writing good HTML code. The reason isn’t obvious right now, but it will be important when we talk about styling our page. (AKA adding pretty colors, fonts, and cool text effects.) More on that in the next module! 

Another extremely common tag you will be using in your websites is the `<h1>` tag. The “h1” is for “Heading 1”. Heading 1 is, by default, the largest heading you have. We have multiple heading tags, `<h1>` through `<h6>`. 

# h1
## h2
### h3
#### h4
##### h5
###### h6

Modify your code such that we have an element with the `<h1>` tag before the `<p>` tag. 

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>Example Web Page</title>
	</head>
	<body>
		<h1> Some heading here </h1>
		<p> Hello World </p>
	</body>
</html>
```
Save and then refresh your page!

Do you see what happened? Now, play around with some of the other headings. 

Another common tag you will be using is the `<ul>` and `<li>` tags. The ul tag defines an unordered list, and each item in that list (between the ul tags) must be surrounded by the `<li>` tag. 

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>Example Web Page</title>
	</head>
	<body>
		<h1> Some heading here </h1>
		<p> Hello World </p>
		<h2> This is a list of my favorite things: </h2>
		<ul>
			<li> Raindrops on roses </li>
			<li> Whiskers on kittens </li>
			<li> Bright copper kettles </li>
			<li> Warm woollen mittens </li>
		</ul>
	</body>
</html>
```

Given that `<ul>` defines an unordered list, what do you think the `<ol>` tag specifies? 

## Self-closing Tags

There are some special tags in HTML that don’t require a closing tag. For example, `<meta>` tags do not require closing tags, nor does the `<img>` tag. The meta tags are extremely important, because they provide the browser with metadata, or important information about the site. Some common meta tags are: 

`<meta name = “author” content = “Your Name Here”> `

`<meta name = “description” content = “Some site description here”> `

These meta tags are pretty self explanatory. They don’t appear on your website, but they provide information to the browser about your website, some of which can be important, especially the description tag. This way, users can read your site description before clicking. 

---

[Click here](https://junior-devleague.github.io/JDLA-Web-Development/morea/3_Basic_HTML/reading-attributes.html) to move on to the fourth reading, “Attributes”.

<br>
