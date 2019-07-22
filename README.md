# Color Layer Generator

A Sass partial to generate background color "layers" as CSS classes

---

Simply add a CSS class to add a background-color. Not efficient (layering elements with JS is better for large sets of colors), but for small sets (colors &lt; 7) this might come in handy!

Note that this is not really built for performance, but just to make layering background colors easily simply by adding CSS classes. This was inspired by [this Stack Overflow question][1].

Usage:

		@import 'path/to/_clg'
    @include gen-layers($params)

Where @params is a list of the format:

    $params: (
      '[class_name]': ([R], [G], [B], [A]),
      ...
    )

See [./examples][2] for a worked example.

[1]: https://stackoverflow.com/questions/57138883
[2]: [./examples/example.html]
