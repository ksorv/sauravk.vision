---
layout: layouts/post.njk
title: The (Not So) Hard CSS - Part 1
metaDesc: This post explains the flow of a HTML document, It helps when you're
  starting out. Later on this just becomes a habit and you get used to it!
socialImage: /images/inline-block.png
date: 2020-07-16T14:44:48.412Z
tags:
  - CSS
  - Document Flow
  - ""
---
# Document Flow

## What is Normal Flow of Documents?

By default, Element boxes are laid out first then with it's content in it, then padding, border and margin around them.

Now, You may ask **what's a element box?**

An element box is nothing but the element's content put in a box and laid out on screen. In below code, there's an example.

Okay, so, There is a CSS property called `display` which is used to tell browser what kind of box that element has! All the elements have default box-types i.e, `<span>` tags are `inline`. Wait, what's that? Look below.

### The `display` Property

There are four main values to the `display` property and those are:

#### block

The element generates a block element box, generating line breaks both before and after the element when in the normal flow. All elements with `display: block;` by default are [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements).

#### inline

The element generates one or more inline element boxes that do not generate line breaks before or after themselves. In normal flow, the next element will be on the same line if there is space. All elements with `display: inline;` by default are [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements).

#### inline-block

The element generates a block element box that will be flowed with surrounding content as if it were a single inline box (behaving much like a replaced element would).

#### none

When set to none, Turns off the display of an element so that it has no effect on layout (_the document is rendered as though the element did not exist_). All descendant elements also have their display turned off.

To have an element take up the space that it would normally take, but without actually rendering anything, use the [visibility](https://developer.mozilla.org/en-US/docs/Web/CSS/visibility) property instead.

---

There is much more to `display` [here](https://developer.mozilla.org/en-US/docs/Web/CSS/display).

---

<iframe height="235" style="width: 100%;" scrolling="no" title="Normal Doc Flow" src="https://codepen.io/sauravkk/embed/OJyoGQv?height=235&theme-id=dark&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/sauravkk/pen/OJyoGQv'>Normal Doc Flow</a> by Saurav kumar
  (<a href='https://codepen.io/sauravkk'>@sauravkk</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### How are elements laid out by default?

By default, a block level element's content is 100% of the width of its parent element, and as tall as its content.

Inline elements are as tall as their content, and as wide as their content. You can't set width or height on inline elements — they just sit inside the content of block level elements.

If you want to control the size of an inline element in this manner, you need to set it to behave like a block level element with display: block; (or even,display: inline-block; which mixes characteristics from both.)

The **normal layout flow** is the system by which elements are placed inside the browser's viewport.

When you do something in vertical mode i.e, sentences run vertically. In normal flow, Blocks are laid horizontally. So blocks boxes run parallel to writing mode.

This is a block here.

Another one here. I think you got what I mean! Refer the image above.


**Block level elements** are generally laid out vertically based on _block flow direction_, which is based on parent's writing mode as shown above, and each one will appear on a new line below the last one, and they will be separated by any margin that is set on them.

**Inline elements** behave differently — they don't appear on new lines; instead, they sit on the same line as one another and any adjacent (or wrapped) text content, as long as there is space for them to do so inside the width of the parent block level element. If there isn't space, then the overflowing text or elements will move down to a new line.

### Important bit:

If two adjacent elements both have the margin set on them and the two margins touch, the larger of the two remains, and the smaller one disappears — this is called **margin collapsing**.

<iframe height="541" style="width: 100%;" scrolling="no" title="Normal Doc Flow" src="https://codepen.io/sauravkk/embed/QWjVPqZ?height=541&theme-id=dark&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/sauravkk/pen/QWjVPqZ'>Normal Doc Flow</a> by Saurav kumar
  (<a href='https://codepen.io/sauravkk'>@sauravkk</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Normal flow is where you begin with any layout: when you create a CSS Layout, you are taking the blocks and causing them to do something other than normal flow.

## Take Advantage Of Document Flow

Okay, I saw this in a post by Smashing Magazine, Taking Advantage, I mean.
Just think how you'll design your page if Browsers started throwing all the elements randomly on your face, You won't know where which one will be placed.

You won't be able to design it!

If for some reason CSS(e.g. someone using a screen reader) or JS does not load, User will still be able to see stuff, cause of Browser's Document flow.

So, Do create elements in good order and make use of the Document Flow.

Create Website like this :=>
Think about Document Structure, Then think about Layout.

**Once you have well-structured document, You'll start thinking about layout. Then, You'll need some elements out of normal order. How you do that?**

---

Next, we'll be taking a look on `float` and `clear` property.
