---
layout: layouts/post.njk
title: Learn CSS in 10 minutes or less!
metaTitle: Learn CSS in 10 minutes or less!
metaDesc: Here comes the next post filed under courses tag, In this I write
  about CSS layouts, Flexbox, And general CSS properties. Get in and Let it
  sink!
socialImage: /images/1561458_7f3b.jpg
date: 2020-05-03T08:02:23.592Z
tags:
  - blog
  - courses
  - free
  - css
  - css-beginners
---
Thanks You for your great response. As you asked for it:

**Here is the CSS3 course for beginners!!!**

- - -

After reading this, you'll know CSS enough, enough to create any layout you want.

## Index

* [What is CSS?](#heading-what-is-css)
* [Linking CSS Files To A HTML](#heading-adding-or-linking-css-file-to-a-html-file.)
* [CSS Syntax](#heading-css-syntax)

  * [CSS Selectors](#heading-css-selectors)
  * [CSS Properties](#heading-css-properties)
* [Resources](#heading-resources)

- - -

## What is CSS?

CSS: Cascading Style Sheets, is a stylesheet language, As the name suggests!\
It is used to describe the presentation of HTML, SVG or xHTML docs.\
CSS describes how any element should be shown on screen, on paper and on other medias.

CSS1 is obsolete. CSS2.1 is used in all browsers by default as per W3C specification. Now, everyone is moving onto CSS3. Let's get started with CSS already.

## Adding or Linking CSS File To A HTML File.

In a Folder Create two files, `styles.css` and `index.html.` Create HTML file as:

```html
Index.html :- 

<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Getting started with CSS</title>
</head>

<body>
    
    <h1>Level one heading</h1>

    <p>A paragraph of text. In the text is a <span>span element</span> 
and also a <a href="http://example.com">link</a>.</p>

    <p>This is the second paragraph. It contains an <em>emphasized</em> element.</p>

    <ul>
        <li class="list" id="one">Item one</li>
        <li class="list two">Item two</li>
        <li>Item <em>three</em></li>
    </ul>
  
  <input type="text" />

</body>

</html>
```

Now, that's something we learned in the last post... I don't think there is anything new in this HTML file that needs to be discussed.

To Add CSS to a HTML file, we use `<link>` tags in the head. How?

```html
<link type="text/css" rel="stylesheet" href="styles.css">

<!-- 
type: Used to tell the browser or parsers the file type, 
Not neccesary but I'd say it is important.

rel: Used to tell the browser or parser what this link tags realtion 
is to the file in which it's included. Very Imp.

href: It tells the location of file we want relative to current file's path.
-->
```

That said, copy and paste this link tag in your HTML file that you created above. Remember to copy it in the head.\
Now, A new question arises! How you know that your CSS file is connected to your HTML file.\
Copy-Paste this in the CSS file:

```css
body {
  background: red;
}
```

Open the HTML File by double clicking it. If you see Red page then everything is fine, else something is wrong.\
**Congrats!** That's your first CSS rule applied to a HTML File. 

Wait, **What's a CSS rule? Here are some important terms!!!**

## **CSS Syntax**

CSS is made of rules that you can write to tell browser what styles to apply. You tell browser something like "I want the background color of my body element to be red" through CSS rules and you get the same.

That thing you copied to CSS, is a CSS rule.

`body {`\
     `background: red;
}`

The Rule is starts with a selector. 

### **CSS Selectors**

A CSS selectors the part of a CSS rule that describes what elements in a document the rule will match. The matching elements will have the rule's specified style applied to them.

In the example above selector is body, i.e, The rule written in it is applied to body tag. Here's a list of all.

```css
/*
CSS Comments are like this. :-)

[Selector Examples]:
*/

.class {
 /* CSS rules here*/ 
}

#id {
 /* CSS rules here*/ 
}

tagsOrElements {
 /* CSS rules here*/ 
}

element.class {
  /* This selects a element with class attribute 'class'.
     [Please, Don't get confued]
  */ 
}

element#id {
  /* This selects a element with id attribute 'id'. */ 
}

.class1 .class2 {
 /* Mind the space when selecting elements with two classes 
    It'll select all the elements having both classes class1 & class2.
    Same with Ids. */
}

[type=text] {
  /* These are attribute selectors, 
     You can select element with some [attr=value] as shown. */
}

* {
 /* Universal Selector, Selects all the elements. 
    Remember *.class is same as .class! */ 
}

selector:active {
  /* Used to select specific state of the selected element.
     Active state is being selected here.
     These are used to apply CSS to elements in a specific state of theirs. */
}

selector:hover {
  /* Most commonly used state selector, Used on <a> tags to change their colors,
     When hovered, or to created animations on hover.*/
}

selector1, selector2 {
  /* This will select both selectors together,*/
}

ul>li{
 /* This is child selector, You can use this to select childs of any element.*/ 
}

/*
We'll discuss some more selectors later on. Dont be scared, they are easy
and also easily available with one google search.
You can check this doc:
https://developer.mozilla.org/en-US/docs/Glossary/CSS_Selector
*/
```

Now, Let's talk about what goes into after a selector selects something.

After a selector, {} comes which contains the properties which needs to be applied and their values.

### CSS Properties

A CSS propertyis a characteristic (like color) whose associated value defines one aspect of how the browser should display the element.

We've **hundreds if not thousands of CSS properties**. And then thousands of values for them. \
I can't and won't discuss all of them here. 

So, Instead I think I'll create a Course where I create some layouts, or Static sites. \
So, You can learn from there. Other than that, CSS Properties:

```css
selector {
  /* I'll list as many as I can or think helpful*/
  
  /* Background */
  background-color: red; /* It sets background color of any element.*/
  background-image: 'https://example.com/image.jpg'; /* bg Image for element*/
  background: whatever color; /* This includes every background prop like color, image etc.*/
  background: url to image; /* Will work as background-image */
  
  /* Border, Instead of long text you gotta specify values ;-) */
  border: sets all border properties in one line;
  border-image: url; /* sets an image as border */
  
  border-radius: border radius of the four rounded corners;
  /* We'll talk about units Soon */
  
  border-left: left border properties in one line;
  border-left-color: border left color;
  border-left-style: border left style;
  border-left-width: border left width;
  
  /* Box props */
  box-shadow: shadow to element;
  box-sizing: box sizing properties; /* Google it or check ref link at end */
  
  color: text-color;
  cursor: cursor type when item hovered;
  display: sets the display type of an element;
  /* Will be covered in next Layout course. */
 
  }

/*
Ok, I got tired!

Check this: https://htmlcheatsheet.com/css/
It contains all the props, Just as I wrote them above.

For specific props
Check this: https://developer.mozilla.org/en-US/docs/Web/CSS/Reference

I'll list some good resources at the end of the post.
*/
```

That's about it for CSS. 

Now, Let's talk about it, As I kind of know you're disturbed by the fact that this post has nothing.

Actually, CSS is just a set of rules that you'll remember with time and if you can't get them in your memory, There is no problem Cause When you use them, You'll get used to them. **Or You can Google them, Anytime you want.**

Nobody can teach you to remember them, but you using it.

Now, You can totally ask: **When I dont know shit about CSS? How can I use it?**

**I'll make some video tutorials where we'll move further by using CSS in real time instead of just memorizing it.**

Okay, Click on these and add them to your bookmarks. 

- - -

## Resources

Please do complete these open source CSS courses:

[Learn CSS Style Guides](https://rscss.io/), How to name classes and stuff?

[Learn CSS Selectors](http://flukeout.github.io/), Check it out. It's too good.

[Learn CSS Layout](http://learnlayout.com/), Don't worry if you can't. I'll teach you later. :-)

- - -

I'll end this post with it. As this post is just meant for beginners. But as I see people are eager to learn.

Also, I'll try to upload a new post every other day, So, We can learn till this CORONA thing ends.

Hey, Take care.

Out,

Saurav.