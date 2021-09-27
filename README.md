# story-jekyll-theme
Jekyll adaptation of the Story website template by [HTML5 UP](https://html5up.net).  Designed for use by those who can write in Markdown, i.e. pretty much anyone.  No prior website building experience required.

## Quickstart

First, [install Jekyll](https://jekyllrb.com/docs/installation/).

Then, clone this repository into a convenient location on your computer.

Next, navigate to the main directory of this project in your terminal and run `jekyll serve`.

Finally, preview the current status of the webpage in your browser at `http://localhost:4000/`.

## Customizing the Webpage

Before proceeding, we recommend you review the different element types provided by the Story theme [here](https://html5up.net/uploads/demos/story/) and the built-in modifiers for each element type.

The following element types are currently supported by this package:
 - Banner
 - Spotlight
 - Gallery
 - Item
 - Form

A webpage designed using this package may be constructed using any number of these elements, in any order.  Each of these elements is represented by a different markdown file in the `_elements` folder.  The order of these elements can be customized in the `_config.yml` file.  How to construct the markdown files which represent each of these elements is described in the following sections:

### Banner

A banner element markdown file contains the following fields in its front matter: 
 - type: Element type (i.e. `banner`)
 - modifiers: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - image: Image file, relative to the `images` directory
 - image_alt: Alternative text for the image file (for slow loading connections)

Markdown text corresponding to the banner element is then inserted after the front matter.

### Spotlight

A spotlight element markdown file contains the following fields in its front matter: 
 - type: Element type (i.e. `spotlight`)
 - modifiers: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - image: Image file, relative to the `images` directory
 - image_alt: Alternative text for the image file (for slow loading connections)

Markdown text corresponding to the spotlight element is then inserted after the front matter.

### Gallery

A gallery element markdown file contains the following fields in its front matter: 
 - type: Element type (i.e. `gallery`)
 - modifiers: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - gallery: ID corresponding to the gallery element

Markdown text corresponding to the gallery element is then inserted after the front matter.

### Gallery Content

Gallery element markdown file content is represented by markdown files in the `_gallery` folder.  Content will be automatically added to the gallery element with a matching ID.  The order of gallery content can be customized in the `_config.yml` file.

Each gallery element markdown file contains the following front matter:


### Items

An items element contains the following fields in its front matter: 
 - type: Element type (i.e. `items`)
 - modifiers: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - items: ID corresponding to the items element

The markdown text corresponding to the items element is then inserted after the front matter.



### Items Content

Items element content is represented by markdown files in the `_items` folder.  Content will be automatically added to the items element with a matching ID.  The order of items content can be customized in the `_config.yml` file.


Items content is represented by markdown files in the `_items` folder.

### Updating Webpage Sections

Webpage content may be updated by modifying the relevant markdown file in the `_sections` folder.  New webpage content may be added by adding new markdown files to the `_sections` folder.

### Updating Gallery Content

### Updating Items Content

### Updating the Webpage Order

To update the webpage layout, 

### Updating Social Media Links

To update the collection of social media links, update the `_config.yml` file with your social media usernames.  Comment out any social media profiles you do not wish to list on your website. 

### Updating Copyright Information

To set the copyright owner for your website, update the `_config.yml` file with your name.

### Setting Contact Information

To update the website t

TODO

## Original README
```
Story by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)


Say hello to Story, a brand new responsive one-pager for HTML5 UP! Inspired by my work
on Carrd*, Story is built to be extremely modular and tweakable, and as such is entirely
built on reusable, insanely customizable elements (like "spotlight" and "gallery") that
can be endlessly duplicated and tweaked into whatever you need to tell your story --
without, in many cases, touching *any* CSS. Check out index-demo.html for an interactive
demo, and index.html for the actual template. Enjoy!

Demo images** courtesy of Unsplash, a radtastic collection of CC0 (public domain) images
you can use for pretty much whatever.

PS: Delete index-demo.html and assets/js/demo.js when you're done messing with the demo
as neither are needed in production :)

(* = my other side project -- carrd.co)
(** = not included)

AJ
aj@lkn.io | @ajlkn


Credits:

	Demo Images:
		Unsplash (unsplash.com)

	Icons:
		Font Awesome (fontawesome.io)

	Other:
		jQuery (jquery.com)
		Scrollex (github.com/ajlkn/jquery.scrollex)
		Responsive Tools (github.com/ajlkn/responsive-tools)
```
