# Inconsistent Line Height with Unitless `line-height` and Percentage `font-size`

This repository demonstrates an uncommon CSS bug related to line height inconsistencies when using a unitless `line-height` value with a percentage-based `font-size`.  The issue is that the unitless `line-height` is relative to the font size, and using a percentage-based font-size introduces variability.  The bug is resolved by adding explicit units (`em`, `rem`, etc.) to the `line-height` property.

## Bug Description
When using `font-size` as a percentage and a unitless `line-height`, unexpected spacing can occur since the unitless `line-height` is relative to the font size, which might vary.

## Bug Solution
Adding explicit units (like `em` or `rem`) to `line-height` resolves the inconsistency, providing predictable spacing regardless of the font size.