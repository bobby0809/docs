---
title: 'index'
attributions:
  - 'Mozilla Developer Network [![cc-by-sa-small-wpd.svg](/assets/thumb/8/8c/cc-by-sa-small-wpd.svg/120px-cc-by-sa-small-wpd.svg.png)](http://creativecommons.org/licenses/by-sa/3.0/us/): [Article](https://developer.mozilla.org/en-US/docs/Web/Guide/API/Gamepad)'
readiness: 'Ready to Use'
relationships:
  applies_to:
    predicate: 'Property of '
    value: apis/gamepad/Gamepad
    href: /apis/gamepad/Gamepad
  return:
    predicate: 'Returns an object of type '
    value: 'unsigned long'
    href: /apis/gamepad/Gamepad
standardization_status: 'W3C Working Draft'
summary: 'The index of the gamepad in the Navigator.'
tags:
  - API_Object_Properties
  - API
  - Gamepad
uri: apis/gamepad/Gamepad/index

---
## Summary

The index of the gamepad in the Navigator.

Property of [apis/gamepad/Gamepad](/apis/gamepad/Gamepad)[apis/gamepad/Gamepad](/apis/gamepad/Gamepad)

## Syntax

**Note**: This property is read-only.

``` js
var result = object.index;
```

## Return Value

Returns an object of type unsigned longunsigned long

## Examples

The Gamepad API provides a function, [Navigator.getGamepads](/dom/Navigator/getGamepads), that returns a list of all devices currently visible to the web page, as an array of Gamepad objects. When a gamepad is connected, this example reports its index, id, number of buttons, number of axes, and when the gamepad data was updated.

``` js
window.addEventListener("gamepadconnected", function(e) {
  var gp = navigator.getGamepads()[e.gamepad.index];
  console.log("Gamepad connected.");
  console.log("Gamepad index:", gp.index);
  console.log("Gamepad id:", gp.id);
  console.log("Gamepad buttons:", gp.buttons.length);
  console.log("Gamepad axes:", gp.axes.length);
  console.log("Gamepad last updated:", gp.timestamp);
});
```

## Related specifications

[W3C Gamepad Specification](https://dvcs.w3.org/hg/gamepad/raw-file/default/gamepad.html)
:   W3C Working Draft
