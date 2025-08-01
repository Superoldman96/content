---
title: -webkit-box-reflect
slug: Web/CSS/-webkit-box-reflect
page-type: css-property
status:
  - non-standard
browser-compat: css.properties.-webkit-box-reflect
sidebar: cssref
---

{{Non-standard_Header}}

The **`-webkit-box-reflect`** [CSS](/en-US/docs/Web/CSS) property lets you reflect the content of an element in one specific direction.

## Syntax

```css
/* Direction values */
-webkit-box-reflect: above;
-webkit-box-reflect: below;
-webkit-box-reflect: left;
-webkit-box-reflect: right;

/* Offset value */
-webkit-box-reflect: below 10px;

/* Mask value */
-webkit-box-reflect: below 0 linear-gradient(transparent, white);

/* Global values */
-webkit-box-reflect: inherit;
-webkit-box-reflect: initial;
-webkit-box-reflect: revert;
-webkit-box-reflect: revert-layer;
-webkit-box-reflect: unset;
```

### Values

- `above`_,_ `below`_,_ `right`_,_ `left`
  - : Are keywords indicating in which direction the reflection is to happen.
- {{CSSxRef("&lt;length&gt;")}}
  - : Indicates the size of the reflection.
- {{CSSxRef("&lt;image&gt;")}}
  - : Describes the mask to be applied to the reflection.

## Formal definition

{{CSSInfo}}

## Formal syntax

{{CSSSyntaxRaw(`-webkit-box-reflect = [ above | below | right | left ]? <length>? <image>?`)}}

## Specifications

Not part of any standard. The standard way to do reflection in CSS is to use the CSS {{CSSxRef("element", "element()")}} function.

## Browser compatibility

{{Compat}}

## See also

- The Apple [documentation](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariCSSRef/Articles/StandardCSSProperties.html).
- The WebKit [specification](https://webkit.org/blog/182/css-reflections/).
