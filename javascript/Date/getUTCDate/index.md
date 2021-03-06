---
title: 'getUTCDate'
attributions:
  - 'Microsoft Developer Network: [Article](http://msdn.microsoft.com/en-us/library/ie/z8d0k600(v=vs.94).aspx)'
compatibility:
  feature: getUTCDate
  topic: javascript
readiness: 'Ready to Use'
summary: 'Gets the day-of-the-month, using Universal Coordinated Time (UTC).'
tags:
  - JS_Basic
  - JS_Method
uri: javascript/Date/getUTCDate

---
## Summary

Gets the day-of-the-month, using Universal Coordinated Time (UTC).

## Syntax

    dateObj.getUTCDate()

## Return Value

Returns an integer between 1 and 31 that represents the day-of-the-month.

## Examples

The following example shows how to use the **getUTCDate** method.

``` js
var date = new Date("1/23/2001");
 document.write(date.getUTCDate());

 // Output: 23
```

## Remarks

The required dateObj reference is a **Date** object. To get the day of the month using local time, use the **getDate** method.

## See also

### Other articles

-   [getDate Method (Date)](/javascript/Date/getDate)
-   [setDate Method (Date)](/javascript/Date/setDate)
-   [setUTCDate Method (Date)](/javascript/Date/setUTCDate)

