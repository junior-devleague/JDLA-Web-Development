---
title: "Attributes"
published: true
morea_id: reading-attributes
morea_summary: "An explanation of HTML attributes"
morea_type: reading
morea_sort_order: 11
morea_labels:
 - HTML
---

# Attributes 

A common self-closing tag is the `<img>` tag. What would a website be without images? We also use CSS to set images, and that will be shown later. But for now, to add images to your site, we’ll use the `<img>` tag inside our HTML documents. 

The image tag has two required _attributes_, `src` and `alt`.

`<img src = “path to image or url link” alt = “some alternate text to display in case image does not load”>`

Attributes provide more information about an html element. Sometimes, certain attributes are required with certain tags, like for `<img>`. Without both the `src` and `alt` attributes and their respective values, the `<img>` tag will not work properly. So, if you just had an `<img>` tag with a `src` written correctly, but no `alt` attribute/value, then your image will not load. 

The value that goes between the **“ ”** in `src` is the _path_ to the image file. If you remember paths from the second module, [Intro to Command Line](https://junior-devleague.github.io/JDLA-Web-Development/modules/intro-to-command-line/), you’ll know that you’re in your project folder, where your index.html file is. However, **you will be saving your images (that you bring, or that you can download off the internet) to your `images` directory**. So, to get to a given image, you would follow the path:

`images/imageNameHere.png`

Your images can be _.png_, _.jpeg_, _.jpg_, or _.gif_ files. Make sure you put in the proper file extension and that your image files follow the file naming conventions, with no spaces in the name. Please try to rename your images short, descriptive titles if you’re downloading them off the internet. 

Also, make sure you keep all images in this class PG. 

Anyway, your image tag should look something like this: 

`<img src = “images/mindlessMeme.png” alt = “Another bizarre, mind-numbing, meme”>`

In the body of your file (_try to remember: what goes inside the body?_) add an image!

The `<meta>` tag has many attributes, such as charset and name. Meta tags also require the use of some attribute(s). 

## Classes and IDs

Two of the most common attributes are `class` and `id`. Knowing how to use them effectively will be crucial to mastering HTML and using it to create professional-looking websites. 

id’s are unique to an element and only used once in the document. 

For example: 

```html
<p id = “aboutDogs”> 
This is a paragraph about dogs. Dogs are cool. Dogs are awesome. Dogs are the best. I love Dogs. Dogs are amazing.
</p>
```

That particular paragraph has an id called “aboutDogs”, and the id tells us that that paragraph is … well, about dogs. Assuming that you’ll have many paragraphs in your website, it’s good to identify the only section where you’ll be talking about dogs. Perhaps you want there to be special glittery effects and background images for that one section, because dogs are special and deserve special recognition. The id is important when we want to select certain sections of our code later on and style/organize them. 

On the other hand, we have classes, which are used to identify multiple elements you expect to all fall under a certain umbrella. 

```html
<p class = “animalDescription”>

Dogs are cool.
I love dogs. 
Dogs are AMAZING!!!!!!

</p>

<p class = “animalDescription”>

Cats are evil.
Cats are manipulative and lazy and self-serving. 
Cats attempt to take over the world. We must not allow that to happen!!

</p>

<p class = “animalDescription”>

Zebras are weird.
From an evolutionary standpoint, I have no clue why they exist.
Their color combination is really ugly. 

</p>

```
All of the paragraphs are descriptions of animals, so we give them the class attribute “animalDescription”. This way, if we wanted to select all the paragraphs describing animals and surround them with a colorful border, we could do that very easily because they have the same class!

You can also combine id’s and classes, and have good, descriptive, HTML code that can easily be styled. 

```html
<p class = “animalDescription” id = “aboutDogs”>

Dogs are cool.
I love dogs. 
Dogs are AMAZING!!!!!!

</p>

<p class = “animalDescription” id = “aboutCats”>

Cats are evil.
Cats are manipulative and lazy and self-serving. 
Cats attempt to take over the world. We must not allow that to happen!!

</p>

<p class = “animalDescription” id = “aboutZebras”>

Zebras are weird.
From an evolutionary standpoint, I have no clue why they exist.
Their color combination is really ugly. 

</p>

```
This way, we can make references to an entire class of elements, as well as specific individual elements. This might seem simple and somewhat pointless, but it’s extremely important that you group and label your elements correctly. You probably won’t see why now, but you will later on! We _will_ be revisiting classes and id’s, so make sure you get into the practice of using them effectively!

## Anchor tags

To close off this reading, we’ll go over anchor tags. There are so many tags with so many attributes out there, that we couldn’t possibly cover them all, so please explore them on your own. 

Anchor tags are how we link people to external sites/resources, or even to other parts of your site. The syntax for anchor tags is: 

```html
<a href = “urlhere”> This is a link </a>
```
`href` is a required attribute for anchor tags. What the above code does is create [clickable links](https://junior-devleague.github.io/JDLA-Web-Development/). 

You can actually create clickable images that link elsewhere by nesting an `<img>` tag inside an anchor tag:

```html
<a href="link here">
<img src="images/devleagueLogo.png" alt="DevLeague Logo">
</a>
```

You can combine id’s or classes with an anchor tag to create _page jumps_, aka jumping from one section of a long page to another section. We won’t show you how to do that here, because we’re just about exceeding reasonable reading length (such that we still have your attention), but you can look up how to do that yourself! 

---

You’re just about ready now to do your first exercise! Using all that you’ve learned so far, you will create a personal profile. [Click here](https://junior-devleague.github.io/JDLA-Web-Development/morea/3_Basic_HTML/experience-profile.html) to go the first experiential learning exercise in this module. 

After you complete the exercise, move on to the fifth reading, [“Linking HTML files”](https://junior-devleague.github.io/JDLA-Web-Development/morea/3_Basic_HTML/reading-linking-files.html).
