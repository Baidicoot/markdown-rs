# Markdown->HTML-rs
This is a simple rust crate to parse (somewhat strict) markdown into HTML, and is partly a rustification of [Parse-MD.js](https://chalarangelo.github.io/parse-md-js/). Currently it can parse most aspects of markdown.
## Accepted syntax:
- Headers are available via the `#` syntax:
```
# H1
## H2
etc...
```
- Emphasis works using both underscores (`_`) and asterixis (`*`):
```
*emphasis*
_also emphasis_
**strong emphasis**
__also strong emphasis__
```
- Lists are available through ordered (`1. etc`) or unordered (`- or *`) syntax:
```
+ This is an unordered List
- As is this

1. But this isn't
2. This is ordered
```
NB. List nesting is unsupported.
- Code is set through backticks and fenced backticks.
- Horizontal breaks are accessed through triple hashes, equals or hyphens.
```
###
===
---
```
- Line breaks are currently unavailable.

## License
`markdown.rs` is licensed under the MIT License.
