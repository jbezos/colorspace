## colorspace

This package provides some tools related to PDF color spaces and color
management. It requires xcolor, which is loaded if it has not been
before.

Currently it supports what I think are the most common tools:

* Spot colors (CMYK and CIE LAB)
* Mixed spot and process colors (up to 4)
* ICC based default CMYK, RGB and Gray spaces
* Overprinting

Currently only pdftex and luatex are supported.  It seems to work with tikz.

For example, to define a spot color, just say something like:

\definespotcolor{foo}{BarTone 555 GN}{.3, .4, .5, .6}

That's all.

### Latest changes

```
* 1.3   Fixes several incompatibilities with pgf/tikz
* 1.2.0 CIE LAB spot colors (including mixed inks with a
        CMYK alternative)
* 1.1.1 is compatible with luatex 0.95
```

License:     MIT

Repository:  https://github.com/jbezos/colorspace

________
Javier Bezos --- http://www.texnia.com

2019-03-25