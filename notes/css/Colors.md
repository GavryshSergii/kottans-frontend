## Color Name Keywords

Color name keywords can be used to set color property values for elements in CSS.

```
h1 {
color: aqua;
}

li {
color: khaki;
}
```

## CSS Color Alpha Values

_Alpha values_ determine the transparency of colors in CSS. Alpha values can be set for both RGB and HSL colors by using
`rgba()` and `hsla()` and providing a fourth value representing alpha. Alpha values can range between `0.0` (totally
transparent) and `1.0` (totally opaque).

The CSS `transparent` value can also be used to create a fully transparent element.

```
.midground {
background-color: rgba(0, 255, 0, 0.5);
}

.foreground {
background-color: hsla(34, 100%, 50%, 0.1);
}

.transparent {
color: transparent;
}
```

## CSS Hexadecimal Colors

CSS colors can be represented in _hexadecimal_ (or hex) notation. Hexadecimal digits can represent sixteen different
values using `0`-`9` and `a`-`f`.

Hexadecimal colors are composed of 6 characters–each group of two represents a value between 0 and 255 for red, green,
or blue. For example `#ff0000` is all red, no green, and no blue.

When both characters of all three colors are repeated, hex colors can be abbreviated to only three values, so `#0000ff`
could also be represented as `#00f`.

```
.red {
color: #ff0000;
}

.short-blue {
color: #00f;
}
```

## CSS HSL Colors

CSS colors can be declared with the HSL color system using `hsl()` syntax. This syntax contains three values: _hue_ (the
color value itself), _saturation_ (intensity), and _lightness_.

Hue values range from 0 to 360 while saturation and lightness values are represented as percentages.

```
.light-blue {
background-color: hsl(200, 70%, 50%);
}
```

## CSS rgb() Colors

CSS colors can be declared with RGB colors using `rgb()` syntax.

`rgb()` should be supplied with three values representing red, green, and blue. These values range can from 0 to 255.

```
.hot-pink {
color: rgb(249, 2, 171);
}

.green {
color: rgb(0, 255, 0);
}
```
