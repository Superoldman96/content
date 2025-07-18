---
title: "Navigator: contacts property"
short-title: contacts
slug: Web/API/Navigator/contacts
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.Navigator.contacts
---

{{APIRef("Contact Picker API")}}{{SeeCompatTable}}{{SecureContext_Header}}

The **`contacts`** read-only property of the
{{domxref("Navigator")}} interface returns a {{domxref('ContactsManager')}} interface
which allows users to select entries from their contact list and share limited details
of the selected entries with a website or application.

## Value

A {{domxref('ContactsManager')}} object. Two successive calls return the same object.

## Examples

The following code checks whether the Contact Picker API is supported.

```js
const supported = "contacts" in navigator && "ContactsManager" in window;
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [A Contact Picker for the Web](https://developer.chrome.com/docs/capabilities/web-apis/contact-picker)
- [Contact Picker API live demo](https://mdn.github.io/dom-examples/contact-picker/)
