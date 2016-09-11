# code-39-font

The code 39 font can be used to render code39 encoded strings.

## available sizes

The font is available in 5 different height to width ratios.
(Usually i use code39_XL)

if you need other height to width ratios, you can generate your own font using the [barcode font generator](test)

| name | height to width ratio | font size to get 1px wide bars |
| --- | --- | --- |
| code39_S | 1:1 | 15px |
| code39 | 2:1 | 30px |
| code39_L | 3:1 | 45px |
| code39_XL | 4:1 | 60px |
| code39_XXL | 5:1 | 75px |

You can download the font in .ttf, .woff, and .svg format.

## install

You can install it as any other font.
To use it as a webfont, you can install with bower:

    bower install --save code-39-font

and the in your .html:

    <link rel="stylesheet" href="bower_components/code-39-font/code39_all.css"/>
    <div class="code_39_XL">*Test*</div>

## usage

Code 39 does not require special encoding. the `*` - character is the start and stop symbol. Only large cap letters can be encoded in code 39, so make sure to `.toUpperCase()` your strings before displaying.
