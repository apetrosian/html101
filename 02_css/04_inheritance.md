# Inheritance

CSS property can be inherited by default ("Inherited: Yes") or not inherited by default ("Inherited: no").

This controls what happens when no value is specified for a property on an element.

## Inherited properties

When no value for an **inherited property** has been specified on an element, the element gets the computed value of that property on its parent element. Only the root element of the document gets the initial value given in the property's summary.

A typical example of an inherited property is the color property. Given the style rules:

```css
p { color: green }
```

and the markup:

```html
<p>This paragraph has <em>emphasized text</em> in it.</p>
```

the words *"emphasized text"* will appear green, since the em element has inherited the value of the color property from the p element. It does not get the initial value of the property (which is the color that is used for the root element when the page specifies no color).

## Non-inherited properties

When no value for an non-inherited property (sometimes called a reset property in Mozilla code) has been specified on an element, the element gets the initial value of that property (as specified in the property's summary).

A typical example of a non-inherited property is the border property. Given the style rules:

```css
p { border: medium solid }
```

and the markup

```html
<p>This paragraph has <em>emphasized text</em> in it.</p>
```
the words "emphasized text" will not have a border (since the initial value of border-style is none).
