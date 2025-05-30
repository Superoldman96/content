---
title: "ARIA: aria-checked attribute"
short-title: aria-checked
slug: Web/Accessibility/ARIA/Reference/Attributes/aria-checked
page-type: aria-attribute
spec-urls:
  - https://w3c.github.io/aria/#aria-checked
  - https://www.w3.org/WAI/ARIA/apg/patterns/checkbox/examples/checkbox/
sidebar: accessibilitysidebar
---

The `aria-checked` attribute indicates the current "checked" state of checkboxes, radio buttons, and other widgets.

> [!NOTE]
> Where possible use an HTML {{htmlelement("input")}} element with `type="checkbox"` and `type="radio"` as these have built in semantics and do not require ARIA attributes.

## Description

The `aria-checked` attribute indicates whether the element is checked (`true`), unchecked (`false)`, or if the checked status is indeterminate (`mixed`), meaning it is neither checked nor unchecked. The `mixed` value is supported by the tri-state input roles of [`checkbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/checkbox_role) and [`menuitemcheckbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/menuitemcheckbox_role).

The `mixed` value is not supported on [`radio`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/radio_role), [`menuitemradio`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/menuitemradio_role), or [`switch`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/switch_role) and elements that inherits from these. The value will be false if `mixed` is set when not supported.

```html
<span
  role="checkbox"
  id="checkBoxInput"
  aria-checked="false"
  tabindex="0"
  aria-labelledby="chk15-label"></span>
<label id="chk15-label">Subscribe to the newsletter</label>
```

The `tabindex` attribute is required to enable focus. JavaScript is required to toggle the `aria-checked` state. And, if this checkbox is part of a submittable form, more JavaScript is required to set a name and a value.

The above could have been written as:

```html
<input type="checkbox" id="chk15-label" name="Subscribe" />
<label for="chk15-label">Subscribe to the newsletter</label>
```

By using the {{htmlelement("input")}} element with `type="checkbox"` instead of ARIA, there is no need for any JavaScript.

## Values

- false
  - : The element supports being checked but is not currently checked.
- true
  - : The element is checked.
- mixed
  - : for [`checkbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/checkbox_role) and [`menuitemcheckbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/menuitemcheckbox_role) only, equivalent to `indeterminate`, indicating a mixed mode value of neither checked nor unchecked.
- undefined (default)
  - : The element does not support being checked.

## Associated roles

Used in roles:

- [`checkbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/checkbox_role)
- [`menuitemcheckbox`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/menuitemcheckbox_role)
- [`menuitemradio`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/menuitemradio_role)
- [`option`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/option_role)
- [`radio`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/radio_role)
- [`switch`](/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/switch_role)

## Associated interfaces

- {{domxref("Element.ariaChecked")}}
  - : The [`ariaChecked`](/en-US/docs/Web/API/Element/ariaChecked) property, part of the {{domxref("Element")}} interface, reflects the value of the `aria-checked` attribute.
- {{domxref("ElementInternals.ariaChecked")}}
  - : The [`ariaChecked`](/en-US/docs/Web/API/ElementInternals/ariaChecked) property, part of the {{domxref("ElementInternals")}} interface, reflects the value of the `aria-checked` attribute.

```js
myHTMLElement.ariaChecked = true;
```

## Specifications

{{Specifications}}

## See also

- [`<input type="checkbox">`](/en-US/docs/Web/HTML/Reference/Elements/input/checkbox)
- [`<input type="radio">`](/en-US/docs/Web/HTML/Reference/Elements/input/radio)
- [`aria-pressed`](/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-pressed)
- [`aria-selected`](/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-selected)
- [Two state checkbox example](https://www.w3.org/WAI/ARIA/apg/example-index/checkbox/checkbox.html) - w3.org
- [Mix-state checkbox example](https://www.w3.org/WAI/ARIA/apg/example-index/checkbox/checkbox-mixed.html) - w3.org
