-webkit-border-vertical-spacing zoom calculation
=============

## Explanation
Using index.html you can see the difference in rounding of values when applying different zoom values to the body.

Values of 1, 1.25, 1.5, 2 etc result in round values for both the div and the table vertical spacing.

However, when more complex rounding is done for values such as 1.1, 1.2, 1.3 etc then the div is round to nearly 4 (usually 3.9..) however the vertical spacing is calculated to some values along way from 4 e.g. zoom of 1.2 sets the value to 3.33..px.

## Recreation

- Chrome Canary 48.0.2542.0
- Safari 9.01

## Issue
https://code.google.com/p/chromium/issues/detail?id=547891
