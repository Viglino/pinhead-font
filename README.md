# <img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEC57-pin.svg" height="40" /> Pinhead-Font
*Icon font set for use with GIS and spatial analysis tools*

[![](https://img.shields.io/npm/v/pinhead-font.svg)](https://www.npmjs.com/package/pinhead-font)
![](https://img.shields.io/npm/dt/pinhead-font.svg)
![](https://img.shields.io/npm/dw/pinhead-font)
![](https://img.shields.io/npm/l/pinhead-font.svg)

I've collected in this repo icons and graphics I've been using in my projects.
Pinhead-Font icons and font theme is designed mainly for GIS applications and web mapping tools. 
They can be easily included in a project using the font or svg images.

[See demo page and examples <img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEC57-pin.svg" height="25" />](https://viglino.github.io/pinhead-font/)

## <img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEBCE-clock_face.svg" height="35" align="left" />Getting started

###  NPM package

Pinhead-Font is availiable on [npm](https://www.npmjs.com/package/pinhead-font):
```console
npm install --save pinhead-font
```
You can access the font or css in the `./font` and `./css` directory of the package.    
The svg sprites are located in the `./dist/pinhead-font.svg` SVG file.

### using Pinhead-Font

You can use Pinhead-Font as a font or as SVG symbols or images.

To use it in a web page, just add the css in your project.
```html
<link href="https://viglino.github.io/pinhead-font/css/pinhead-font.css" rel="stylesheet" />
```
Then use an inline element with a class prefixed with `pin-` to add a new icon.    
<img src="https://github.com/Viglino/pinhead-font/blob/main/svg/geometric_shapes/uEB23-map_pin_with_dot.svg" height="30" />
<img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEC73-shopping_basket.svg" height="30" />
```html
<!-- prefix: fg - icon name: poi -->
<i class="fg-poi"></i>
<!-- using a <span> is more semantically correct but a little bit verbose. -->
<span class="fg-polyline-pt"></span>
```
Or use it as an svg sprite (svg sprites are inlocated in the `./dist/pinhead-font.svg` file):    
<img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEC73-shopping_basket.svg" height="30" />
```html
<svg class="pinhead-font fg-3x"><use xlink:href="path/to/dist/pinhead-font.svg#pin-shopping_basket" /></svg>
```

## <img src="https://github.com/Viglino/pinhead-font/blob/main/svg/hand_tools/uEB44-brick_trowel.svg" height="35" align="left" />Contributing
Please use the [GitHub issue tracker](https://github.com/Viglino/pinhead-font/issues) to ask for new features 
or create a pull request.    
Font is created from the files in the `./svg` folder, you only have to create a new file in this folder. 
Use the `./templates/template.svg` template to create a new icon.  
You can add a new glyph in the [pinhead-font.json](https://github.com/Viglino/pinhead-font/blob/main/pinhead-font.json) file with a theme and search tags 
(other fields will be filled automatically).

Your contribution will be published under [Pinhead-Font license](https://github.com/Viglino/pinhead-font/blob/main/LICENSE.md) as per [GitHub's terms of service](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license).

If you wan't to build the font and create the dist, use the build script (run `npm install` to install the dev dependencies before):
```console
npm run build
```
Use a local server (http://localhost:8181/) to see result on the page:
```console
npm start
```


## <img src="https://github.com/Viglino/pinhead-font/blob/main/svg/misc/uEC73-shopping_basket.svg" height="35" align="left" />Licenses

**Pinhead-Font is licensed under [Apache-2.0](https://github.com/Viglino/pinhead-font/blob/main/LICENSE-APACHE.md)**    
Copyright (c) 2021 Jean-Marc Viglino

[Pinhead-Font](https://viglino.github.io/pinhead-font/) is free, open source, and GPL friendly. 
You can use it for commercial projects, open source projects, or really almost whatever you want.
[Read full Pinhead-Font license](https://github.com/Viglino/pinhead-font/blob/main/LICENSE.md)

Dual-license can be used for each specific part:
* Pinhead-Font **font** is licensed under the [SIL OFL 1.1 License](./LICENSE-OFL.md)
* **Icons** and **SVG** files are licensed under the [CC0 License](./LICENCE)
* **Codes** and all non font or icon files are licensed under the [MIT License](./LICENSE-MIT.md)
