---
title: 'getRangeAt'
attributions:
  - 'Mozilla Developer Network [![cc-by-sa-small-wpd.svg](/assets/thumb/8/8c/cc-by-sa-small-wpd.svg/120px-cc-by-sa-small-wpd.svg.png)](http://creativecommons.org/licenses/by-sa/3.0/us/): [[Selection.getRangeAt](https://developer.mozilla.org/en-US/docs/Web/API/Selection.getRangeAt) Article]'
  - 'Microsoft Developer Network: [[getRangeAt Method](http://msdn.microsoft.com/en-us/library/ie/ff975177(v=vs.85).aspx) Article]'
readiness: 'Ready to Use'
relationships:
  method_of:
    predicate: 'Method of '
    value: dom/Selection
    href: /dom/Selection
  return_type:
    predicate: 'Returns an object of type  '
    value: Range
    href: /dom/Selection
standardization_status: 'W3C Working Draft'
summary: 'Returns a specified Range from a selection. The Range is specified by an index and cannot be greater than the number that is returned by rangeCount. '
tags:
  - API_Object_Methods
  - DOM
uri: dom/Selection/getRangeAt

---
## Summary

Returns a specified Range from a selection. The Range is specified by an index and cannot be greater than the number that is returned by rangeCount.

Method of [dom/Selection](/dom/Selection)[dom/Selection](/dom/Selection)

## Syntax

``` js
var range = selObj.getRangeAt(/* see parameter list */);
```

## Parameters

### index

 Data-type
:   Number

 The zero-based index of the range to return. A negative number or a number greater than or equal to rangeCount will result in an error.

## Return Value

Returns an object of type RangeRange

The range object that will be returned.

## Examples

``` js
var ranges = [];

var selObj = window.getSelection();

for(var i = 0; i < selObj.rangeCount; i++) {
 ranges[i] = selObj.getRangeAt(i);
}
/* Each item in the ranges array is now
 * a range object representing one of the
 * ranges in the current selection */
```

## Notes

### Remarks

Currently only Gecko supports multiple or disjointed selections.

### Syntax

### Standards information

-   [HTML5 A vocabulary and associated APIs for HTML and XHTML](http://go.microsoft.com/fwlink/p/?linkid=221374), Section 7.6.1
