# connect-fonts-droidserif

Droid Serif fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-droidserif");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/droidserif-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/droidserif-bold,droidserif-bolditalic,droidserif-italic,droidserif/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* droidserif-bold
* droidserif-bolditalic
* droidserif-italic
* droidserif

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/droidserif-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin

5. Set your CSS up to use the new font by using the "Droid Serif" font-family.
```
    body {
      font-family: 'Droid Serif', 'sans-serif', 'serif';
    }
```

## Font Info
Droid Serif

* Description: Droid Serif is a contemporary serif typeface family designed for comfortable reading on screen. Droid Serif is slightly condensed to maximize the amount of text displayed on small screens. Vertical stress and open forms contribute to its readability while its proportion and overall design complement its companion Droid Sans.
* Copyright: Digitized data copyright © 2007, Google Corporation.
* Trademark: Droid is a trademark of Google and may be registered in certain jurisdictions.
* Designer URL: http://www.ascendercorp.com/typedesigners.html 
* Vendor: Ascender Corporation
* Vendor URL: http://www.ascendercorp.com/

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-droidserif
* Repo: https://github.com/shane-tomlinson/connect-fonts-droidserif.git
* Bugs: https://github.com/shane-tomlinson/connect-fonts-droidserif/issues

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 2.0 of the Apache

  http://www.apache.org/licenses/LICENSE-2.0

