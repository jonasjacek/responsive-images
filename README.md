# Responsive Images

**Information, resources and sample implementations of responsive images in HTML and CSS in conjunction with [Cloudinary](https://cloudinary.com/) for art direction.**

---

## Table of contents

<!-- vim-markdown-toc GFM -->

* [Responsive images in HTML](#responsive-images-in-html)
  * [Device-pixel-ratio-based selection](#device-pixel-ratio-based-selection)
  * [Viewport-based selection](#viewport-based-selection)
  * [Art direction-based selection](#art-direction-based-selection)
* [Responsive images in CSS](#responsive-images-in-css)
* [Terminologies](#terminologies)
* [Examples](#examples)
* [Documentation](#documentation)
  * [Introduction](#introduction)
  * [Prerequisites](#prerequisites)
  * [Web Standards](#web-standards)
  * [Browser Support](#browser-support)
  * [Cloudinary](#cloudinary)
  * [General](#general)
* [Mirrors](#mirrors)
* [Warranty and Liability](#warranty-and-liability)
* [Licenses](#licenses)
* [Contribute](#contribute)

<!-- vim-markdown-toc -->

---

## Responsive images in HTML

Responsive images in HTML are a method for providing the browser with multiple image sources for an image slot. The browser selects an image, depending on display density, size of the image element in the page, or any number of other factors. 

The following selection methods are available:


### Device-pixel-ratio-based selection

**Resolution switching for displaying an image with a fixed size while supporting different screen resolutions.**

The `img` element's `sizes` and `srcset` attributes are used in conjunction with the `x` descriptor.

Use this selection method if the rendered size of the image is fixed (e.g. by `height` and `width` attributes on the `img` element. The images in `srcset` only vary in their intrinsic width to support different resolutions (image content is identical).

Browsers which do not support the `sizes` and `srcset` attributes will ignore them and load the image referenced in the `src` attribute.


### Viewport-based selection

**Resolution switching for displaying different sizes of an image.**

The `img` element's `sizes` and `srcset` attributes are used in conjunction with the `w` descriptor. 

The images only vary in their size (image content is identical).

Browsers which do not support the `sizes` and `srcset` attributes will ignore them and load the image referenced in the `src` attribute.


### Art direction-based selection

**Resolution switching for displaying different image sizes and contents.**

The `picture` elements `source` element's `media` and `srcset` attributes reference different image sources for the browser to choose from. 

The images may not only vary in their size but also image content may not be identical.

Browsers which do not support the `picture` and `source` elements will ignore them and load the image referenced in the `img` elements `src` attribute.


## Responsive images in CSS

Responsive images in CSS can be implemented with the help of media queries (`@media`). The browser picks the image that matches the media query.

Browsers which do not support `@media` will ignore the rules.


---

## Terminologies

* **Art direction**  
  Images in the `srcset` show different images suitable for different space allocations.
* **CSS pixel**  
  A measurement unit. CSS pixels are hardware pixels divided by pixel density.
* **Device pixel ratio (DPR)**  
  Ratio between hardware pixels and logical pixels.
* **Hardware pixel**  
  An individual dot of light in the display.
* **Intrinsic width**  
  The real size of an image.
* **Physical pixel**  
  See _Hardware pixel_.
* **Pixel density**  
  The number of pixels present per inch on a display. The density is measured in Pixels Per Inch (PPI).
* **Resolution switching**  
  All images in the `srcset` show the same thing but contain different numbers of pixels.
* **Software pixel**  
  See _CSS pixel_.


## Examples

Examples of different usages of responsive images can be found in `/examples`.


## Documentation

### Introduction

Introductions to responsive images on the Web:

* https://html.spec.whatwg.org/multipage/images.html#images
* https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images

### Prerequisites

The following concepts should be understood:

* https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries
* https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units

### Web Standards

Web Standards that relate to responsive images on the Web:

* https://html.spec.whatwg.org/multipage/grouping-content.html#the-figure-element
* https://html.spec.whatwg.org/multipage/grouping-content.html#the-figcaption-element
* https://html.spec.whatwg.org/multipage/embedded-content.html#the-picture-element
* https://html.spec.whatwg.org/multipage/embedded-content.html#the-img-element

### Browser Support

* https://caniuse.com/css-mediaqueries
* https://caniuse.com/picture
* https://caniuse.com/srcset

### Cloudinary

Links to the Cloudinary documentation, which describe techniques used in this repository:

* https://cloudinary.com/documentation/image_transformations
* https://cloudinary.com/documentation/image_transformation_reference#crop_parameter

### General

Links to useful resources:

* https://caniuse.com/
* https://en.wikipedia.org/wiki/Pixel_density

## Mirrors

You can find this repository at:
* GitLab  
  [https://gitlab.com/jonasjacek/responsive-images](https://gitlab.com/jonasjacek/responsive-images)
* GitHub  
  [https://github.com/jonasjacek/responsive-images](https://github.com/jonasjacek/responsive-images)

## Warranty and Liability
[Responsive Images](https://gitlab.com/jonasjacek/responsive-images) is a small, private project. The author makes absolutely no claims and representations to warranties regarding the accuracy or completeness of the information provided. However, you can use the information in this repository AT YOUR OWN RISK.

## Licenses

<span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">Responsive Images</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://gitlab.com/jonasjacek/responsive-images" property="cc:attributionName" rel="cc:attributionURL">Jonas Jacek</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. Permissions beyond the scope of this license may be available upon <a xmlns:cc="http://creativecommons.org/ns#" href="https://www.jonas.me/contact" rel="cc:morePermissions">request</a>.

Atomic size parts of contents were taken from the [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/docs/Web), which is written by Mozilla Contributors. These contents are also licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-SA)](https://creativecommons.org/licenses/by-sa/4.0). 

The [bullseye icon](https://commons.wikimedia.org/wiki/File:IPA_Unicode_0x0298.svg) was created by [Martin Kozák](https://commons.wikimedia.org/wiki/User:Martin_Koz%C3%A1k), who released the work into the [public domain](https://en.wikipedia.org/wiki/en:public_domain).


## Contribute

Found a mistake? [Open an issue](https://gitlab.com/jonasjacek/responsive-images/-/issues) or [send a merge request](https://gitlab.com/jonasjacek/responsive-images/-/merge_requests). Want to help in another way? [Contact me](https://www.jonas.me/contact).
