# Fonts installed on the ScanMeFindMe QR generator server

You can insert any fonts in the template and they will be available when you generate QR codes in SVG format.
However for PNG, PDF, PS formats the fonts have to be installed on the server.

## How to use fonts in the template:

1. Add the `<style>` section and import necessary fonts.

2. In the respective `<text>` tag add `font-family` and `font-size` attributes

Beware that many fonts do not have full UTF-8 support. Make sure to select the fonts that
can display the characters from your language. It is possible to specify multiple fonts in the
`font-family` attribute.

## Example of the template

This template loads Roboto and Ubuntu fonts and specifies both of them

```svg
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="1000" height="1300" viewBox="0 0 1000 1300">
    <defs>
        <style>
            @import url('https://fonts.googleapis.com/css2?family=Roboto:ital@0;1&amp;family=Ubuntu&amp;display=swap');
        </style>
    </defs>
    <rect fill="none" stroke="#000000" stroke-width="20" stroke-linejoin="round" stroke-dashoffset="" fill-rule="nonzero" id="svg_3" x="10" y="10" width="980" height="1280" stroke-opacity="1"/>
    <rect fill="#c0c0c0" stroke="none" stroke-width="1" stroke-linejoin="round" stroke-dashoffset="" fill-rule="nonzero" id="qr" x="100" y="100" width="800" height="800" fill-opacity="1"/>
    <text x="500" y="1125" font-size="100" text-anchor="middle" id="caption" font-weight="500"
          font-family="Ubuntu, Roboto">
        SCAN ME
    </text>
</svg>
```

## Google fonts

The following [google fonts](https://fonts.google.com) are installed on ScanMeFindMe. Follow the links
to preview them and generate `<style>` tag.
Remember that you need to replace `&` with `&amp;` in the fonts URLs in order to use them inside SVG.

* [Roboto](https://fonts.google.com/specimen/Roboto?preview.text_type=custom)
* [Roboto Mono](https://fonts.google.com/specimen/Roboto+Mono?preview.text_type=custom)
* [Open Sans](https://fonts.google.com/specimen/Open+Sans?preview.text_type=custom)
* [Open Sans Condensed](https://fonts.google.com/specimen/Open+Sans+Condensed?preview.text_type=custom)
* [Lobster](https://fonts.google.com/specimen/Lobster?preview.text_type=custom)
* [Ubuntu](https://fonts.google.com/specimen/Ubuntu?preview.text_type=custom)
* [Ubuntu Mono](https://fonts.google.com/specimen/Ubuntu+Mono?preview.text_type=custom)

## How to add more fonts

To request a new font please create an issue in this repository.
