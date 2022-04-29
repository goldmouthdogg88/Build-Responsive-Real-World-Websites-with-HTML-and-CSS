# Section 3: CSS Fundamentals

### 22. Introduction to CSS

What CSS is, and common terminology.

What is CSS?

Cascading Style Sheets, one of the core technologies of the web

CSS describes the visual style and presentation of the content written in HTML

CSS consists of countless properties that developers use to format the content: properties about font, text, spacing, layout, etc.

```css
h1 {
  color: blue; // property: value
}
```

CSS always starts with a selector, then we can apply some style to it. Each style we can call a declaration, property, value
between curly braces are the declaraction block. all this together makes up a CSS rule.

### 24 Styling Text

```css
h1 {
  color: blue;
  font-size: 26px;
}

h2 {
  font-size: 40px;
  font-family: sans-serif;
}

p {
  font-size: 22px;
  font-family: sans-serif;
  line-height: 1.5;
}

li:last-child {
  font-style: italic;
}

li:nth-child(2, [odd, even]) {
  color: red;
  /* Use_Case:: Useful for styling alternating tables */
}

article p:first-child {
  color: red; // nothing happend, is first p, but not first child
}
```

descendent selector

### 29. Styling Hyperlinks

How to style hyperlinks using pseudo classes

```

<!-- not a good practice, we should target a pseudo classes of anchor so that we can target different states. -->
a {
    color: #1098ad;
}

a:link {
    color: #1098ad;
    text-decoration: none;
}

<!-- Many sites display links differently if they have been visited, we can actaully group similar rules together! But for now lets keep them separate -->

a:visited {
    color: #1098ad;
}

a:hover {
    color: orangered;
    font-weight: bold;
    text-decoration: underline dotted orangered;
}
<!-- State when we actaully click the link -->
a:active {
    background-color: black;
    font-style: italic;
}

```
