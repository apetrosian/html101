# Layout

## Block elements

The **block elements** are often used as a layout tool, because it can easily be positioned with CSS.

#### Semantic elements

HTML5 offers new semantic elements that define different parts of a web page:

- `<header>`
Defines a header for a document or a section

- `<nav>`
Defines a container for navigation links

- `<section>`
Defines a section in a document

- `<article>`
Defines an independent self-contained article

- `<aside>`
Defines content aside from the content (like a sidebar)

- `<footer>`
Defines a footer for a document or a section

- `<details>`
Defines additional details

- `<summary>`
Defines a heading for the `<details>` element

#### Float property

The **float** CSS property specifies that an element should be taken from the normal flow and placed along the left or right side of its container, where text and inline elements will wrap around it.

Here is an example of layout positioning using float:

```css
nav {
  float: left;
  width: 160px;
}

section {
  margin-left: 160px;
}
```

> The size of the blocks can be also specified in **precent** instead of pixel. This approach commonly called fluid layout.


## Tables

The `<table>` element was **not designed** to be a layout tool.

The purpose of the `<table>` element is to display **tabular data only**.


## Media Queries

The `@media` rule is used to define different style rules for different media types/devices.

Media queries look at the capability of the device, and can be used to check many things, such as dimensions of the viewport, device orientation and more.


```html
<!-- CSS media query on a link element -->
<link rel="stylesheet" media="(max-width: 800px)" href="example.css" />

<!-- CSS media query within a stylesheet -->
<style>
@media (max-width: 600px) {
  .sidebar {
    display: none;
  }
}
</style>
```

[Using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

## Flexbox

The **CSS3 Flexible Box**, or **flexbox**, is a layout mode providing for the arrangement of elements on a page such that the elements behave predictably when the page layout must accommodate different screen sizes and different display devices.

For many applications, the flexible box model provides an improvement over the block model in that it does not use floats, nor do the flex container's margins collapse with the margins of its contents.

[Using CSS flexible boxes](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes)

[A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
