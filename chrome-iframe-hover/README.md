Chrome IFrame Overlap Bug
=========================

Steps:
1. Hovering on item in the iframe.
1. Move the mouse slowly onto the overlapped element from parent to a point
where you are no longer above the iframe.
1. Expect the hovered item in the iframe to lose the hovered style. THIS DOES NOT HAPPEN.

Recreated in:
- Chrome 37.0.2062.94
- Chrome 39.0.2141.0 canary (64-bit)

Chrome bug opened:
https://code.google.com/p/chromium/issues/detail?id=409601
