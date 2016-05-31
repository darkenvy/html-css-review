# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>
</body>
</html>

```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
An img tag displays a image file while a div is a block element that fills the container.
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Inline CSS takes presidence over priority. It is bad practice as it is not scalable 
or easy to modify when projects get large.

Internal style sheets are also bad practice as making modifications require modifying
the .html file.

External style sheets are the proper way to manage CSS as it is scalable and easily
restyled site-wide.
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
/* This will select all div tags and give it a round border */
div {
  border-radius: 50%;
}

/* This will select all p tags that have a parent of a 'header' class and change the
font size to 18 pixels */
.header p {
  font-size: 18px;
}

/* Selects the class footer and moves it to the bottom of the parent element flush (0px) */
.footer {
  position: absolute;
  bottom: 0;
}

/* the class splash-image recieves a background image of an ocean and aligns the size
to be fit horizontally with the rag being vertically. */
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* when class emelents called ninja are hovered over, change the font color to black
and hide the element */
.ninja:hover {
  display: none;
  color: black;
}
```

