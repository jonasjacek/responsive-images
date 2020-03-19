# Responsive Images

**Information, resources and sample implementations of responsive images in HTML and CSS in conjunction with [Cloudinary](https://cloudinary.com/) for art direction.**

## Introduction

### Responsive images in HTML

Responsive images in HTML are a method for providing the browser with multiple image sources in the `img` element's `srcset` attribute. The browser picks an image, depending on display density, size of the image element in the page, or any number of other factors.

### Responsive images in CSS

Responsive images in CSS can be implemented with the help of media queries (`@media` and `@import`).

Examples of different usages of responsive images can be found in `/examples`.

## Terminologies

* Art direction  
  Images in the `srcset` show different images suitable for different space allocations.
* Resolution switching  
  All images in the `srcset` show the same thing but contain different numbers of pixels.
* **CSS Pixels**  
  CSS Pixels are hardware pixels divided by pixel density:  
  CSS Pixels = Hardware Pixels / Pixel density

| Product | Pixel density |
| ------ | ------ |
| My first computer | 1 |
| Macbook Pro | 2 |
| Samsung Galaxy S8+ | 4 |

* **intrinsic width**  
  The real size of an image

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

### Cloudinary

Links to the Cloudinary documentation, which describe techniques used in this repository:

* https://cloudinary.com/documentation/image_transformations
* https://cloudinary.com/documentation/image_transformation_reference#crop_parameter

### General

Links to useful resources:

* https://caniuse.com/

## Mirrors

You can find this repository at:
* GitLab  
  [https://gitlab.com/jonasjacek/responsive-images](https://gitlab.com/jonasjacek/responsive-images)
* GitHub  
  [https://github.com/jonasjacek/responsive-images](https://github.com/jonasjacek/responsive-images)

## Warranty and Liability
[Responsive Images](https://gitlab.com/jonasjacek/responsive-images) is a small, private project. The author makes absolutely no claims and representations to warranties regarding the accuracy or completeness of the information provided. However, you can use the information in this repository AT YOUR OWN RISK.

## License

<span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">Responsive Images</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://gitlab.com/jonasjacek/responsive-images" property="cc:attributionName" rel="cc:attributionURL">Jonas Jacek</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. Permissions beyond the scope of this license may be available upon <a xmlns:cc="http://creativecommons.org/ns#" href="https://www.jonas.me/contact" rel="cc:morePermissions">request</a>.

Atomic size parts of contents were taken from the [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/docs/Web), which is written by Mozilla Contributors. These contents are also licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-SA)](https://creativecommons.org/licenses/by-sa/4.0). 


## Contribute

Found a mistake? [Open an issue](https://gitlab.com/jonasjacek/responsive-images/-/issues) or [send a merge request](https://gitlab.com/jonasjacek/responsive-images/-/merge_requests). Want to help in another way? [Contact me](https://www.jonas.me/contact).
