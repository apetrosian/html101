# CSS

Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language.

## How to add styles to the page

There are three common ways for adding styles to the HTML page.

**External Style Sheet**

Included as an external file using `<link>` element inside the `<head>` section. File must be saved with `.css` extension.

```html
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
```

**Internal Style Sheet**

Defined within the `<style>` element, inside the `<head>` section.

```html
<head>
  <style>
    .text-red {
      color: red;
    }
  </style>
</head>
```

**Inline Styles**

To use inline styles, add the style attribute to the relevant element.

```html
<p style="color:red;">I want to be red.</p>
```
