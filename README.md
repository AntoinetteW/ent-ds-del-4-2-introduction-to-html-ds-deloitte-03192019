
# An Introduction to HTML

## Introduction

HyperText Markup Language (HTML) is the language of the web! It is the way that you take content you would like to share and describe it in a way that a browser can understand and display. Every web page you've ever visited uses HTML to contain the content, and it's important to understand a little bit about what a web page looks like so you'll be able to effectively scrape the content from it.

## Objectives
You will be able to:
* Explain what HTML is and why it's important
* Read a basic HTML document
* Create a simple HTML website 

## HTML Syntax

```html
<p>Hello World</p>
```

Elements, like our `p` tags above, won't be displayed in the browser. Instead,
they affect how the content itself is displayed. Technologists might say that
the tags "affect how the content is rendered by the browser."

We can also alter any number of attributes inside of the opening tags. For
example, the `a` element, which is used for links, has an `href` attribute to
specify the destination address of the link. If we wanted to link to
www.flatironschool.com, we could do so as follows:

```html
<a href="http://www.flatironschool.com">Flatiron School</a>
```

This would render as:

[Flatiron School](http://www.flatironschool.com)

We can also nest elements inside of each other. To have a link displayed as a
separate paragraph, we could nest an `a` element inside of a `p`.

```html
<p>This <a href="http://www.google.com">link</a> will be a part of a separate paragraph.</p>
```

## Basic HTML Document Structure

All HTML documents begin with a "doctype declaration" tag, which tells our web
browser which version of HTML to use. HTML is a language that is currently
evolving &mdash; just like English. When we open "Romeo and Juliet," our
expectation is that the "doctype" is "Elizabethan English." In the same way
"Elizabethan English" has changed to a more modern form, HTML 1.0 was
_essentially_ the same as modern HTML5 but had some tags we don't use any more
and was lacking some tags we use often today.

Since it's not wrapping any content, our doctype declaration doesn't require a
closing tag. To use HTML5, the current up-to-date version, we can simply
declare `<!DOCTYPE html>`.

```html
<!DOCTYPE html>

```

Next, we add an opening and closing `html` tag. This tells the web browser to
interpret everything inside the tags as HTML code.

```html
<!DOCTYPE html>
<html>


</html>
```

Every HTML page is made up of two primary sections: a `head` and a `body`. The
`head` element contains metadata about the HTML document and other information
for the browser, while the `body` element contains the actual content.

```html
<!DOCTYPE html>
<html>
    <head>
        <!-- metadata about the HTML document as a whole -->

    </head>

    <body>
        <!-- content of our page will be here! -->

    </body>
</html>
```

## Comments

Let's also take a brief moment to recognize how to add comments into an HTML
document.  These won't get rendered to the browser at all: they're just helpful
notes for the author.

```html
<!-- NYC Pizza is world-famous, cheap, and loved by both vermin and human like! -->
<p>Top 5 Pizza Places in NYC</p>
```

## Common HTML Elements

We've already looked at some common HTML elements, such as `a` and `p`. Let's
take a look at some more HTML elements.

## Headers

HTML gives us access to different header elements, ranging from `h1` to `h6`,
with `h1` being the largest and `h6` being the smallest.

```html
<h1>Dogs!</h1>
<h3>Why Dogs are Great</h3>

<h6>Different Breeds</h6>
```

In addition to changing how the text is displayed, search engines use headers
to help determine what a web page is about. Remember, as Avi pointed out, when
we provide _semantic_ markup, machines can infer the "main points" of a page. A
well structured article will generally have its principal arguments bracketed
by low-number header tags -- this very document does exactly that!

## Images

We can embed images on our web pages using the `img` element. The `img` element
doesn't have a closing tag. The `src` attribute tells the browser where to find
the image. The `alt` attribute will be displayed if an image can't be loaded,
and also describes the image to search engines.

The `alt` tag presents a moment to talk about an important principle behind Tim
Berners-Lee's vision for the Web: it is _inclusive_. If you're using assistive
technologies because you have a sight impairment, it's helpful to know what's
being displayed. If you're in a remote community where internet access is
expensive, you might choose to disable images and only pay to download those
which you _absolutely need_. So while an `img` will inject an image and "work,"
honoring the Web's vision for openness and inclusivity requires that we provide
the `alt` tag as well.

`<img src="URL_TO_IMAGE" alt="Picture of a Dog">`

## Lists

Some other useful HTML elements are lists. We can make bulleted, or unordered
lists, using opening and closing `ul` tags. Inside, we can nest an `li`, or
"list item" element for each item on our list.

```html
<h5>My Favorite Things in No Particular Order</h5>
<ul>
    <li>Coffee</li>
    <li>Vinyl Records</li>
    <li>Pickling</li>
</ul>
```

This would render as:

____

<h5>My Favorite Things in No Particular Order</h5>
<ul>
    <li>Coffee</li>
    <li>Vinyl Records</li>
    <li>Pickling</li>
</ul>
____

We can also make a numbered, or ordered list, using an `ol` tag.

```html
<h5>Top 5 Pizza Places in NYC</h5>
<ol>
    <li>DiFara Pizza</li>
    <li>Lucali's</li>
    <li>Sal and Carmine's</li>
    <li>Juliana's</li>
    <li>Joe's</li>
</ol>
```
Would render as:

____

<h5>Top 5 Pizza Places in NYC</h5>
<ol>
    <li>DiFara Pizza</li>
    <li>Lucali's</li>
    <li>Sal and Carmine's</li>
    <li>Juliana's</li>
    <li>Joe's</li>
</ol>
____

## Your Turn!

OK, now that we've introduced a number of tags, it's your turn! 

### Getting Set Up
There are two ways you can start to create an HTML web page.
1. Create a file on your laptop with a `.html` file extension (a good name might be `index.html`). Open the file with your favorite text editor, save your changed, then use the File-Open menu option in your web browser to open that local file in the browser.
2. If you don't have a favorite text editor or are not sure how to create, edit, save and open the file, you could also use a third party website that allows you to write HTML and view the results - all online. One popular example is [CodePen](https://codepen.io/pen/).

### Start with the basics

Start by creating a simple website. Remember the `doctype`, `html` tag and the `head` and `body` tags within it. In the head set the `title` tag to set how the page will be described in the browser tab, and then in the body, put an `h1` title, a smaller `h2` title, a couple of `p`aragraphs of text and a `li`st of bulleted items!

### Extra Credit (1)
Make your web page longer. Add three additional headings with at least 3-4 paragraphs of content under each (if you don't want to type the content, you could always [generate some lorem ipsum](https://www.lipsum.com/). Now see if you can find out how to create an anchor tag around each of the headings. Then add a bulleted list to the top of the page with the three headings and a link to each one (hint, you may have to Google a little bit to figure this out).

### Extra Credit (2)
Pick five extra tags from [here](https://www.w3schools.com/tags/), and incorporate them into your web page. If you run into a lot of trouble with a given tag, feel free to move along to another one.


## Summary


Welcome to the world of the web! In this lesson, you learned about HTML and how web pages are structured, and got a little practice creating your own HTML file.
