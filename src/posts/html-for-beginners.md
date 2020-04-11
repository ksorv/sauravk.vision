---
title: Learn HTML5 in 10 Minutes!
metaTitle: HTML5 course For Beginners
metaDesc: I'm making this, cause when I started I grew tired of seeing the same
  shit everywhere. Every course started with so called HTML Basics. So, here
  they are! After this, you'll know HTML enough, enough to create whatever you
  want.
date: 2020-04-10T00:00:00.000Z
tags:
  - blog
  - courses
  - free
  - html
  - html-beginner
metaDescription: HTML5 course for beginners, Totally FREE. I grew tired of all
  these courses having the same HTML5 basics, So I made some courses which will
  teach you HTML, CSS, Javascript fundamentals all in place, and for FREE!
socialImage: /images/html5.jpg
---
**Here is the HTML5 course for beginners!**

I'm making this, cause when I started I grew tired of seeing the same shit everywhere. Every course started with so called **HTML Basics**. So, here they are!

Now, after this If I saw any of you seeing any other Html basic course, **I'll kill you**. After this, you'll know HTML enough, enough to create whatever you want.

- - -

## Index

* [What is HTML?](/posts/html-for-beginners/#heading-what-is-html)
* [HTML Elements](/posts/html-for-beginners/#heading-html-elements)
* [HTML Tags](/posts/html-for-beginners/#heading-html-tags)
* [HTML Attributes](/posts/html-for-beginners/#heading-html-attributes)
* [HTML Comments](/posts/html-for-beginners/#heading-html-comments)
* [White Spaces In HTML](/posts/html-for-beginners/#heading-white-spaces-in-html)
* [Special Characters in HTML](/posts/html-for-beginners/#heading-special-characters-in-html)
* [Wrapping Up](/posts/html-for-beginners/#heading-wrapping-up)
* [References](/posts/html-for-beginners/#heading-references)
* [End Of The Course](/posts/html-for-beginners/#heading-end-of-the-course)

- - -

## What is HTML?

**HTML** -> Stands for ***Hyper Text Markup Language***

That means it's markup, not a programming language. **PERIOD**. It is the most basic thing you'll need to create a web page and is fundamental to almost all the front end frameworks.

You are supposed to be using CSS and JS with this markup to create websites.

## How to write and serve HTML?

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>This is title of the page! As shown on the tab of browser</title>
  </head>
  <body>
    <p>This is content of the page!</p>
  </body>
</html>
```

Let's demystify it!

1. `<!DOCTYPE html>` : No one really cares about them, and they are just a historical artifact that needs to be included for HTML to work right. `<!DOCTYPE html>` is what counts as a valid doctype; that's all.
2. `<html></html>` : This `<html>` element tells web browser that inside of it is all the content of the entire page. It is also known as the root element.
3. `<head></head>` : This element contains everything that isn't shown to the user but your web page needs it for it's configuration and data. For example: The meta data, CSS files, Page title, favicon are all linked inside of the head.
4. `<meta for="something">` : In meta tags you specify the data which is used by search engines, and other social medias to get your sites info like Description, Content, Language etc.
5. `<title></title>` : The `<title>` element  sets the title of your page, which is the title that appears in the browser tab the page.
6. `<body></body>` : The `<body>` element(one in a HTML doc) contains *all* the content that you want to show to web users.

Copy the code above and create a file through any code editor or notepad with name `index.html`, paste the code you copied form here. Save it! Now double click on it. You'll see that it opens in the browser.

It's your very first HTML file, Viola!!! Now you can try putting the tags you learned before into this file and refresh the web page to see the changes. Later someday I'll teach you servers and stuff which serve it through www.

For now let's see what HTML has?

## HTML Elements!

HTML uses something that is called a element which is made of tags, attributes and content. Almost all the HTML elements have opening and closing tags. Let's see some elements:

`<p>This is a Paragraph tag</p>`

The above element is a p tag, used to create paragraphs as one that you are reading. Notice it has `<p>` at start and `</p>` at the end, these are called opening and closing tags respectively.  The text between is content. Let's see another example:

`<img src="/path/image.jpg" />`

This is an image tag, it has no closing tag. But a simple `/>`.  Img elements are **empty elements,** needs no content and/or closing tags.

A good picture from [MDN Docs](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started) is:

![HTML element](/images/html-element.png "A HTML element with p tag")

That said now you know what html is made of, let's teach you some tags and stuff.

## HTML Tags

**I've a pen, on which when you click you'll see HTML and its preview on the side. You don't need to understand anything, Right now!** Just have a look!

There are may be 100 HTML tags that you'll learn someday. I wont write all of them here, as there is no need for that.  I'll list out those which are handy and used most:

* `<hX>`This is a heading!`</hX>` You can use X=1,2...,7.. whatever.
* `<p>`This is a paragraph tag`</p>`
* `<img src="./path/image.jpg" alt="This is alt text"/>`
* `<strong>`This is strong tag, used to bold the text.`</strong>`
* `<em>`This tag is used for italic text.`</em>`
* `<span>`Generally used where you want to style text.`</span>`
* `<br />` This is a break tag, used to get something into new line.
* `<ul><li>`This is an item in unordered list.`</li></ul>`
* `<ol><li>`This is an item in ordered list.`</li></ol>`
* `<a href="https://sauravk.vision" target="_blank">A anchor tag</a>`
* `<input type="text">` This is an input element.
* `<form>`This is form element.`</form>`
* `<button>`This is a button`</button>`

That's all I'll tell you for now. Now see this and check how all of these looks, you can also change anything to see preview.

<iframe height="265" style="width: 100%; border: 2px solid black; " scrolling="no" title="HTML" src="https://codepen.io/sauravkk/embed/preview/abvzYpb?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy"> See the Pen <a href='https://codepen.io/sauravkk/pen/abvzYpb'>HTML</a> by Saurav kumar (<a href='https://codepen.io/sauravkk'>@sauravkk</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## HTML Attributes

Attributes are markup that contains extra information about the elements. Like their class, styles and stuff...

As MDN Docs says about it:

An attribute should have:

* A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
* The attribute name, followed by an equal sign.
* An attribute value, with opening and closing quote marks wrapped around it.

Here are some use case:

```html
<p class="paragraph">This is a paragraph.</p>
<!-- The above element has an class attribute with value paragraph -->

<a href="https://example.com" target="_blank">This is a link</a>
<!-- href attribute with value, and a target attribute with value -->
```

## HTML Comments

You can use comments in HTML, to make your code more readable for others and for yourself. As:

`<!-- This is a comment -->.`

This is how you use comments:

```html
<form>
  <!-- For user's full name -->
  <input type="text" placeholder="Enter your name" >
  <!-- For user's email -->
  <input type="email" placeholder="Enter your email" >
  <!-- this button invokes the submit func instead of default behaviour -->
  <button type="button" onClick="onSubmit()">Submit</button>
</form>
```

## White Spaces in HTML

See these examples, first:

```html
<p>This is a paragraph.</p>

<p> This           is         a
  
 spaced          Paragraph   with empty lines.</p>
```

So, HTML parser reduces each white space(**space**, **tabs** and even **line** **breaks**) in between to one space. You can use however much of white space you can, to increase the readability if your code. It is good to use readable code so others can understand your code. 

But what if you really want to have some spaces in your page? Then, you can use special characters. Lets see.

## References: Special Characters in HTML

As you see HTML tags use `<>/` etc. So, how can we write them. If i do something like:

`<p>This is a <p> element</p>`

Then, it has two opening p tags but one closing tag, but I wanted to use one of the tags in the content. Silly browser thought that it's a new p element. So, how do i go about using one?

HTML has some special characters for this kind of thing and they are:

```brainfuck
|------------|-------|
| You'll Use |  For  |
|------------|-------|
|   &lt;     |   <   |
|   &gt;     |   >   |
|   &quot;   |   "   |
|   &apos;   |   '   |
|   &amp;    |   &   |
|------------|-------|

So, for:
<p>In HTML, you define a paragraph using the <p> element.</p>

You'll use:
<p>In HTML, you define a paragraph using the &lt;p&gt; element.</p>
```

## Wrapping up

This was everything about HTML that you needed to learn. You can constantly practice writing HTML and/or creating sites, what will follow is that you'll start to remember all these things like *tags* and *attributes*. So, we're done with HTML. Check out other [Courses](/tags/courses), such as on [CSS basics](/posts/css-for-beginners), [JS basics](/posts/js-for-beginners) and what not.

## References

Do check [MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML) docs, they are full of information on everything web. Other than that, Check my [posts](/archive).

- - -

## End Of The Course

Hopefully this course helped you learn something, which will help on your projects. If it does, or if you got questions, [drop me a tweet](https://twitter.com/sauravkhdoolia), or [DM me](https://instagram.com/beardeddev), because I’d love to listen!