# story-jekyll-theme
Jekyll adaptation of the [Story website template](https://html5up.net/uploads/demos/story/) by [HTML5 UP](https://html5up.net).  Designed for use by those who can write in Markdown, i.e. pretty much anyone.  No prior website building experience required.

- [Quickstart](#quickstart)
- [Customizing](#customizing)
  * [Banner Element](#banner-elements)
  * [Spotlight Element](#spotlight-elements)
  * [Gallery Element](#gallery-elements)
    + [Gallery Images](#gallery-images)
  * [Items Element](#items-elements)
    + [Items](#items)
  * [Social Media](#social-media)
  * [Copyright](#copyright)

## Quickstart

 1. [Install Jekyll](https://jekyllrb.com/docs/installation/).
 2. Clone this repository into a convenient location on your computer.
 3. Navigate to the main directory of this project in your terminal and run `jekyll serve`.
 4. Preview the current status of the webpage in your browser at `http://localhost:4000/`.

## Customizing

Webpages designed using this template may be constructed using any number of Banner, Spotlight, Gallery, Item, and/or Form elements, in any order.  Each element is highly customizable, so a large number of different webpage layouts are possible. For an introduction to each of these elements, and to their various customizations, see https://html5up.net/uploads/demos/story/.

In the context of this Jekyll-based template, each of these elements is represented by a different markdown file in the `_elements` folder.  The markdown file corresponding to each element may be created as described in the following sections.  The order of each of these elements on the webpage can be customized in the `_config.yml` file.

### Banner Elements

A banner element markdown file contains the following fields in its front matter: 
 - `type`: Element type (i.e. `banner`).
 - `modifiers`: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/#reference-banner).
 - `button_link`: Button link.  If this field is omitted, the button is not displayed.
 - `button_text`: Button text.
 - `button_options`: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - `image`: Image file, relative to the `images` directory
 - `image_alt`: Alternative text for the image file (for slow loading connections)

Markdown text corresponding to the banner element is then inserted after the front matter.

### Spotlight Elements

A spotlight element markdown file contains the following fields in its front matter: 
 - `type`: Element type (i.e. `spotlight`)
 - `modifiers`: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/#reference-spotlight)
 - `button_link`: Button link.  If this field is omitted, the button is not displayed
 - `button_text`: Button text.
 - `button_options`: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - `image`: Image file, relative to the `images` directory
 - `image_alt`: Alternative text for the image file (for slow loading connections)

Markdown text corresponding to the spotlight element is then inserted after the front matter.

### Gallery Elements

A gallery element markdown file contains the following fields in its front matter: 
 - `type`: Element type (i.e. `gallery`)
 - `modifiers`: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/#reference-gallery)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - gallery: ID corresponding to the gallery element

Markdown text corresponding to the gallery element is then inserted after the front matter.

#### Gallery Images

The content associated with each gallery element image is represented by markdown files in the `_gallery` folder.  Each image will be automatically added to the gallery element with a matching ID.  The order of images can be customized in the `_config.yml` file.

Each gallery element image markdown file contains the following fields in its front matter:
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - image: Full image file, relative to the `images` directory
 - thumb: Thumbnail image file, relative to the `images` directory
 - image_alt: Alternative text for the image file (for slow loading connections)
 - gallery: ID corresponding to the gallery element

Markdown text corresponding to the image is then inserted after the front matter.

### Items Elements

An items element contains the following fields in its front matter: 
 - type: Element type (i.e. `items`)
 - modifiers: Element modifiers, as described [here](https://html5up.net/uploads/demos/story/#reference-items)
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - items: ID corresponding to the items element

Markdown text corresponding to the items element is then inserted after the front matter.

#### Items

The content associated with each items element item is represented by markdown files in the `_items` folder.  Each item will be automatically added to the items element with a matching ID.  The order of items can be customized in the `_config.yml` file.

An items element contains the following fields in its front matter: 
 - button_link: Button link.  If this field is omitted, the button is not displayed
 - button_text: Button text.
 - button_options: Button modifiers, as described [here](https://html5up.net/uploads/demos/story/)
 - items: ID corresponding to the items element

Markdown text corresponding to the item is then inserted after the front matter.

### Form Elements

A contact form element contains the following fields in its front matter:
 - type: Element type (i.e. `items`)
 - action: Action associated with the contact form. (e.g. https://formspree.io/youremail@mail.com)

Markdown text corresponding to the item is then inserted after the front matter.

### Social Media

To customize the collection of social media links, update the `_config.yml` file with your social media usernames.  Comment out any social media profiles you do not wish to list on your website. 

### Copyright

To set the copyright owner for your website, update the `_config.yml` file with the copyright-owner.

## Deployment

For instructions on how to deploy the resulting content online, see the [Jekyll documentation](https://jekyllrb.com/docs/deployment/).  For example, [this webpage]() has been deployed from this repository using Github Actions.

NOTE: GitHub Actions is required to deploy to GitHub Pages because [GitHub won't update their version of Jekyll](https://github.com/github/pages-gem/issues/651).
