---
title: NavigationTransition.finished
slug: Web/API/NavigationTransition/finished
page-type: web-api-instance-property
tags:
  - API
  - Experimental
  - finished
  - History
  - Navigate
  - Navigation
  - Navigation API
  - Property
  - Read-only
  - Reference
  - Scroll
  - Traversal
browser-compat: api.NavigationTransition.finished
---

{{APIRef("Navigation API")}}{{seecompattable}}

The **`finished`** read-only property of the
{{domxref("NavigationTransition")}} interface returns a {{jsxref("Promise")}} that fulfills at the same time the {{domxref("Navigation/navigatesuccess_event", "navigatesuccess")}} event fires, or rejects at the same time the {{domxref("Navigation/navigateerror_event", "navigateerror")}} event fires.

## Value

A {{jsxref("Promise")}} that resolves to `undefined`.

## Examples

```js
async function cleanupNavigation() {
  await navigation.transition.finished;
  // Navigation has completed successfully
  // Cleanup any ongoing monitoring
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Modern client-side routing: the Navigation API](https://developer.chrome.com/docs/web-platform/navigation-api/)
- [Navigation API explainer](https://github.com/WICG/navigation-api/blob/main/README.md)
- Domenic Denicola's [Navigation API live demo](https://gigantic-honored-octagon.glitch.me/)
