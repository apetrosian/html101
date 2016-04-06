# Attributes

HTML elements can have **attributes**

Attributes provide **additional information** about an element

Attributes are always specified in the **opening tag**


## Boolean attributes

The presence of a boolean attribute on an element represents the true value, and the absence of the attribute represents the false value.

If the attribute is present, its value must either be the empty string or a value that is an ASCII case-insensitive match for the attribute's canonical name, with no leading or trailing whitespace.

As an example, take the disabled attribute, which you can assign to form input elements if you want them to be disabled (greyed out) so the user can't enter any data in them.

```html
<input type="text" disabled="disabled">
```

As shorthand, it is perfectly allowable to write this as follows:

```html
<input type="text" disabled>
```

## Single or double quotes?

Double quotes are the most common in HTML, but this is purely a matter of style, and you can feel free to chose which one you prefer.
