# Selectors

## Type

CSS type selectors match elements by node name.

```css
  h1 {
    border-bottom: 1px solid black;
  }
```

One of the common use cases for this selectors is to reset default browser specific styles, for example:

```css
  html, body {
    margin: 0px;
    padding: 0px;
  }
```

## ID

Use `id` attribute to assign **ID Selector** to the element. The ID name must be **unique** in the document.

```html
  <div id="content">...</div>
```

In CSS selector ID starts with `#`

```css
#content {
  background-color: #EEE;
}
```

> Usually IDs are rarely used to apply styles, better practice is to use **class selectors** instead.

## Class

Use `class` attribute to assign **Class Selectors** to the element.

```html
  <p class="error">...</p>
```

In CSS selector ID starts with `.` (period).

```css
.error {
  color: red;
}
```

Multiple elements in a document can have the same class value. In the same time single element can has multiple classes.

```html
  <p class="error critical">...</p>
```

## Attribute

You are not restricted to the two special attributes, class and id. You can specify other attributes by using square brackets. Inside the brackets you put the attribute name, optionally followed by a matching operator and a value.

```css
  /* Selects all .btn elements with a "disabled" attribute. */
  .btn[disabled] {
    color: grey;
  }

  /* Selects secure links. */
  a[href^="https://"] {
    color: green;
  }
```

## Pseudo-class and pseudo-element

A CSS pseudo-class is a keyword added to selectors that specifies a special state of the element to be selected. For example `:hover` will apply a style when the user hovers over the element specified by the selector.

```css
a:hover {
  color: black;
}
```

Just like pseudo-classes, **pseudo-elements** are added to selectors but instead of describing a special state, they allow you to style certain parts of a document. For example, the `::first-line` pseudo-element targets only  the first line of an element specified by the selector.

---

To see a complete list of selectors, visit [CSS3 Selectors working spec](http://www.w3.org/TR/selectors/#selectors).
