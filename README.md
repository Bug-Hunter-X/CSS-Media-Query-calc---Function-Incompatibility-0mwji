# CSS Media Query calc() Function Incompatibility

This repository demonstrates an uncommon CSS bug related to using the `calc()` function within media query conditions. Some browsers have limited or no support for this, leading to inconsistencies in how styles are applied.

## Bug Description
The issue arises when using `calc()` within a media query's conditional statement, such as `@media (max-width: calc(100vw - 100px))`. While this might work in modern browsers, older ones may not correctly parse or apply the styles within this media query.

## Solution
The solution involves avoiding the use of `calc()` directly within the media query condition.  Instead, use JavaScript or a CSS preprocessor to dynamically set the media query breakpoint.