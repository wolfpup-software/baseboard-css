# Baseboard-css

Keep styles consistent between Firefox, Webkit, and Chromium browsers.

## How to use

Copy `./baseboard.css` into a project.

## Applied styles

`Baseboard` removes default:
- paddings
- margins
- borders
- text-alignments
- list styles

Deprecated elements are ignored.

Fonts are assuemd to be styled by the user eventually. Some visually significant correlation to `font-size` is more accessible than the lack of a correlation.

## Why another stylesheet?

`Baseboard` directly references browser code. I can't guarantee other stylesheets do but this one does.

This stylesheet is also limited in scope and focused on a small set of properties. I can't guarantee other stylesheets are but this one is.

## References

`Baseboard` uses the following default stylesheets:
- [firefox](https://searchfox.org/mozilla-central/source/layout/style/res/html.css)
- [webkit](https://github.com/WebKit/WebKit/blob/main/Source/WebCore/css/html.css)
- [chromium](https://chromium.googlesource.com/chromium/blink/+/master/Source/core/css/html.css)

## License

Baseboard is released under the BSD 3-Clause License.
