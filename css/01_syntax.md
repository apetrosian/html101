# Syntax

The CSS syntax reflects this goal and its basic building blocks are:

- The **property** which is an identifier, that is a human-readable name, that defines which feature is considered.

- The **value** which describe how the feature must be handled by the engine. Each property has a set of valid values, defined by a formal grammar, as well as a semantic meaning, implemented by the browser engine.

## CSS declarations

Setting CSS properties to specific values is the core function of the CSS language.

A property and value pair is called a **declaration**, and any CSS engine calculates which declarations apply to every single element of a page in order to appropriately lay it out, and to style it.

```css
{
  color: red;
  line-height: 16px;
}
```

## CSS rulesets

CSS allows this by associating conditions with declarations blocks. Each (valid) declaration block is preceded by a **selector** which is a condition selecting some elements of the page. The pair selector-declarations block is called a **ruleset**, or often simply a **rule**.

```css
div, p {
  margin: 0px;
  padding: 0px;
}
```

## @ (At) Rule

An at-rule is a CSS statement beginning with an at sign, `@` and followed by an identifier.

Following example tells the CSS engine to include an external style sheet for print:

```css
@import url("print.css") print;
```

### Nested at-rules
A subset of nested statements, which can be used as a statement of a style sheet as well as inside of conditional group rules.

```css
@font-face {
  font-family: "San Francisco";
  src: url("SanFrancisco.ttf");
}
```
Describes the aspect of an external font to be downloaded.
