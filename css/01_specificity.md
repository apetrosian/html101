# Specificity

Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.

Specificity is based on the matching rules which are composed of **CSS selectors** of different sorts.


### How is it calculated?

- Every selector has its place in the specificity hierarchy.

- There are four distinct categories which define the specificity level of a given selector: inline styles, IDs, classes and elements.

- When selectors have an equal specificity value, the latest rule is the one that counts.

- When selectors have an unequal specificity value, the more specific rule is the one that counts.



### Selector Types

The following list of selector types is by increasing specificity:

- Type selectors (e.g., `h1`) and pseudo-elements (e.g., `:before`).

- Class selectors (e.g., `.example`), attributes selectors (e.g., `[type="radio"]`) and pseudo-classes (e.g., `:hover`).

- ID selectors (e.g., `#example`).

Universal selector `*`, combinators (`+`, `>`, `~`) and negation pseudo-class `:not()` have no effect on specificity. (The selectors declared inside `:not()` do, however.)

`Inline styles` added to an element always overwrite any styles in external stylesheets and thus can be thought of as having the highest specificity.


### The !important exception

When an `!important` rule is used on a style declaration, this declaration overrides any other declarations. Although technically `!important` has nothing to do with specificity, it interacts directly with it.

Using `!important` is **bad practice** and should be avoided because it makes debugging more difficult by breaking the natural cascading in your stylesheets.

When two conflicting declarations with the `!important` rule are applied to the same element, the declaration with greater specificity will be applied.
