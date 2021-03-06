---
title: 'activeElement'
notes:
  - 'Needs spec reference, example'
readiness: 'In Progress'
relationships:
  applies_to:
    predicate: 'Property of '
    value: dom/shadowdom/ShadowRoot
    href: /dom/shadowdom/ShadowRoot
  return:
    predicate: 'Returns an object of type '
    value: Element
    href: /dom/shadowdom/ShadowRoot
standardization_status: 'W3C Editor''s Draft'
summary: 'Represents the currently focused element in the shadow tree.'
tags:
  - API_Object_Properties
  - API
  - DOM
  - Shadow_DOM
  - Needs_Examples
uri: dom/shadowdom/ShadowRoot/activeElement

---
## Summary

Represents the currently focused element in the shadow tree.

Property of [dom/shadowdom/ShadowRoot](/dom/shadowdom/ShadowRoot)[dom/shadowdom/ShadowRoot](/dom/shadowdom/ShadowRoot)

## Syntax

**Note**: This property is read-only.

``` js
var result = element.activeElement;
```

## Return Value

Returns an object of type ElementElement

On getting, the attribute must return the currently focused element in the shadow tree or null, if there is none.

