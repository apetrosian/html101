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



## Flexbox

[A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
