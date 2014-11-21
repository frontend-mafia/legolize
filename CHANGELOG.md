# v0.3.7

## Breaking changes

No breaking changes

## Bugfixes
 - fixed .height-calculatedFromFontSize() used in textbox.less;
 - removed display: none; from .ListGroup-itemBody();

# v0.3.6

## New features

Media query variables have been added to variables.less

## Breaking changes

This version has a breaking changes when it comes to Grid system, see below:

## Grid

See changes in pull Requests [ #25](https://github.com/frontend-mafia/legolize/pull/25), [ #27](https://github.com/frontend-mafia/legolize/pull/27)

### New features

- Now possible to generate an entire grid system for each media query using .makeGridColumns() which will loop through and create columns.
- Now possible to create column width for multiple media queries ex: .gridColumnWidth(4) and .gridColumnWidth(4, tablet)
- Responsive class names are now supported, Issue: [ #16](https://github.com/frontend-mafia/legolize/issues/16) 

### Breaking changes

- No longer can we &:extend column modifiers (only .Grid-col), now we use .gridColumnWidth(x) mixin 

# v0.3.5

## Breaking changes

No breaking changes

## Bugfixes

### Textbox
  - Fixes cursor alignment on chrome
  ([#19](https://github.com/frontend-mafia/legolize/issues/19))

# v0.3.4

## Breaking changes

### Form
  - Removed .Form-icon and created .Form-item--withIcon modifier instead.
  ([#23](https://github.com/frontend-mafia/legolize/pull/23))

# v0.3.3

## Breaking changes

### Alert
  - Removed caret descendant because we already have a lego for carets.
  ([#15](https://github.com/frontend-mafia/legolize/issues/15))

### Panel
  - Variable renaming border now configurable
  ([#12](https://github.com/frontend-mafia/legolize/issues/12))

## Bug fixes

## Features

### Alert
  - Added cancel button as descendant
