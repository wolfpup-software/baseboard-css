# Baseboard-css

Tiny reset stylesheet for Firefox, Webkit, and Chromium browsers.

## How to use

Copy `./baseboard.css` into a project.

## Applied styles

`Baseboard` changes a handful of css properties outside the responsibility of `layout` and `typography`.

The following properties are resolved to their corresponding values on all elements:
- `padding: 0`
- `margin: 0`
- `border: none`
- `text-alignment: start`
- `list-style: none`

## Questions

### Why another stylesheet?

`Baseboard` directly references browser code. I can't guarantee other stylesheets do but this one does.

This stylesheet is limited in scope and focused on a small set of properties. I can't guarantee other stylesheets are but this one is.

### Why not typography?

From experience, typography is assumed to be styled eventually and wholeheartedly.

Until then, I believe some visually significant correlation to `font-size` or `line-height` is more accessible than the absence of a correlation.

### Why not inputs?

There differences between input elements across browsers eventually spill into the responsibility of `typography` and `layout`.

Many vertical alignment pains stem from `line-height` and `font-size` properties.

### Why not wildcard selectors?

The point of `baseboard` is to be targeted and concise. Wildcards have neither of those properties. 

I believe wildcard selectors _do not_ take a performance hit worth avoiding their use. The `*` is pretty cool.

## References

`Baseboard` uses the following default stylesheets:
- [firefox](https://searchfox.org/mozilla-central/source/layout/style/res/html.css)
- [webkit](https://github.com/WebKit/WebKit/blob/main/Source/WebCore/css/html.css)
- [chromium](https://chromium.googlesource.com/chromium/blink/+/master/Source/core/css/html.css)

## License

`Baseboard-css` is released under the BSD 3-Clause License.
