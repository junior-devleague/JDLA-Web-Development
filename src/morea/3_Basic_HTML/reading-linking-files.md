---
title: "Linking HTML files"
published: true
morea_id: reading-linking-files
morea_summary: "An explanation of how to link multiple files together in HTML"
morea_type: reading
morea_sort_order: 12
morea_labels:
 - HTML
 - navigation
---

# Linking HTML files

Now that you know how an HTML document should be structured, we can make more HTML documents and link them together. When you go to a website, there’s several links that you click on to take you to other pages in the website. Those other pages are literally other HTML pages, which you link together at the top of your document. 

When you make another HTML document for a different page, a good place to start is to copy over the index.html and make changes to headings and content as needed. 

However, at the top of every page, you should have a navigation bar. A nav bar uses the `<nav>` tags to indicate that it’s your page navigation, and within the `<nav>` tags, you have an unordered list whose elements are links to other pages in the website. 

```html
<nav>
	<ul>
		<li> <a href = “index.html” title = “Home” class = “active”> Home</a></li>
		<li> <a href = “about.html” title = “About our wonderful site”> About</a></li>
		<li> <a href = “contact.html” title = “Contact us!”> Contact</a></li>
	</ul>
</nav>
```

The `class = “active”` indicate that you’d like to indicate that the active link is index.html. For every HTML document, the link that has `class = active` should be one whose href is the same as its name. 

So: 

	The index.html file should have “class = active” on <a href = “index.html> 
	The about.html file should have “class = active” on <a href = “about.html>
	The contact.html file should have “class = active” on <a href= “contact.html”>

This is because if you’re on that page, that means you’ve clicked that link, so that page is the active link! 

Also, you usually want your nav bar to be at the beginning of your document, before any of the content. It should be one of the first elements that goes inside of the body! 

---

Given all of this, please go on to the [second exercise](link here) in Experiential Learning, to test your understanding of basic HTML syntax. Then, continue to the [third exercise](link here), where you will be asked to link files together using what you’ve just learned!

After the exercises, move on to the final reading of this module, [“Special Media and Self-Directed Learning”](https://junior-devleague.github.io/JDLA-Web-Development/morea/3_Basic_HTML/reading-special-media.html).

