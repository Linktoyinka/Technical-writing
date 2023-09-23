---
title: "Styling Images Like a Pro with CSS: Unleashing the Power of "aspect-ratio", "object-fit", and "object-position""
datePublished: Fri Sep 22 2023 17:00:31 GMT+0000 (Coordinated Universal Time)
cuid: clmuulfz4000309mpbovz24s8
slug: styling-images-like-a-pro-with-css-unleashing-the-power-of-aspect-ratio-object-fit-and-object-position
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1695455692141/96414970-2dca-4ebe-9451-d1435243af70.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1695455716720/0705acfb-b776-4b66-8bf0-ef5960fd7863.jpeg
tags: css, web-development, html5, beginners, frontend-development

---

In web development, crafting captivating web experiences is paramount. Image styling with CSS is at the core of this endeavor. This guide delves into CSS, focusing on `aspect-ratio` `object-fit` and `object-position` to empower designers to create visually engaging web projects.

## Introduction

In the realm of web design, images are not just visual elements; they are powerful storytellers and attention-grabbers. Crafting an engaging and visually pleasing website often hinges on how well you can style your images. CSS provides a multitude of tools for this purpose, but in this guide, we will focus on three essential CSS properties that can truly transform your image styling game: `aspect-ratio` `object-fit` and `object-position`

## Prerequisites

* Familiarity with HTML.
    
* Basic knowledge of CSS.
    
* Familiarity with integrated development environment (IDE) and terminal/command line for running code.
    

## Understanding `aspect-ratio`

The CSS property 'aspect-ratio' lets you set the width-to-height ratio of an image. This implies that regardless of how the viewport size changes, the picture will automatically resize to the aspect ratio that has been defined for it. The aspect ratio is used to compute automatic sizes and other layout operations.

At least one of the box sizes must be specified for the aspect ratio to have any effect. If no width or height values are given, the aspect ratio will have no impact.

### Syntax

```css
aspect-ratio: 4 / 2;
aspect-ratio: 1;

/* fallback to 'auto' for replaced elements */
aspect-ratio: auto 3/4;
aspect-ratio: 9/6 auto;

/* Global values */
aspect-ratio: inherit;
aspect-ratio: initial;
aspect-ratio: revert;
aspect-ratio: revert-layer;
aspect-ratio: unset;
```

### Aspect-ratio values

1. `aspect-ratio: 4 / 2;`: The width and height share ratio is shown in value '4/2'. A numerator '4' defines the width, and a denominator '2' is used for height. It's got a width of 4 and a height of 2. A fraction of 2 from the numerator shall be allocated to the height, which is set automatically on any viewport.
    
2. `aspect-ratio: 1;`: When a single value (an integer) is passed for this CSS property, height, and width will share the same value, giving a perfect square shape.
    
3. `auto`: The element's default value has no preferred aspect ratio and should size itself naturally. As a result, when replacing items having an inherent aspect ratio, such as photos, use that aspect ratio.
    

### Examples

%[https://codepen.io/linktoyinka/pen/ZEVJRNr?editors=1100] 

### Browser support

| Browser | Supported |
| --- | --- |
| Chrome | Yes |
| Firefox | Yes |
| Safari | Yes |
| Edge | Yes |
| Internet Explorer | Yes |
| Opera | Yes |

## Understanding `object-fit`

The `object-fit` attribute specifies how an element responds to its content box's height and width. It is designed to be used in combination with the `object-position` property for photos, movies, and other embeddable media types. `Object-fit`, when used alone, allows us to crop an inline picture by providing seamless control over how it squishes or stretches within its box.

### Syntax

```css
object-fit: contain;
object-fit: fill;
object-fit: cover;
object-fit: scale-down;
object-fit: none;

/* Global values */
object-fit: inherit;
object-fit: initial;
object-fit: revert;
object-fit: revert-layer;
object-fit: unset;
```

### Object-fit values

1. `contain`: Increases or decreases the image's size to fill the box while keeping its `aspect-ratio`.
    
2. `fill`: This is the default value, which stretches the image to fill the content box regardless of `aspect-ratio`.
    
3. `cover`: The picture will fill the height and breadth of its box, retaining its `aspect-ratio` but frequently cropping the image in the process.
    
4. `scale-down`: In order to find the smallest tangible object size, the image will compare the difference between `none` and `contain`.
    
5. `none`: The image will remain its original size, whatever the parent's height and width.
    

### Example

%[https://codepen.io/linktoyinka/pen/gOZxNrr?editors=1100] 

### Browser support

| Browser | Supported |
| --- | --- |
| Chrome | Yes |
| Firefox | Yes |
| Safari | Yes |
| Edge | Yes |
| Internet Explorer | Yes |
| Opera | Yes |
| Internet Explorer | No |

## Understanding `object-position`

When employing an `object-fit` property, such as `object-fit: cover;` By cropping out some of the images, the image tends to zoom in to fit the parent container. The CSS property `object-position` is used to align any selected element within the box that contains it, such as images `<img>`.

```css
img {
  object-position: right top;
}
```

### Syntax

The property takes in two values, where the first value is for the horizontal alignment and the second value is for the vertical alignment. These two values can be defined in percentage (%), pixel (px), and CSS-registered keywords (top, left, right, bottom, and center).

### Values

```css
/* Positional values */
object-position: 50% 50%; /* default position */
object-position: right bottom;
object-position: 20px 95px;
object-position: center 20px; /* mix and match */
object-position: 60% top; /* mix and match */

/* Global values */
object-position: inherit;
object-position: initial;
object-position: unset;
```

### Examples

%[https://codepen.io/linktoyinka/pen/eYbVBQp?editors=1100] 

### Browser support

| Browser | Supported |
| --- | --- |
| Chrome | Yes |
| Firefox | Yes |
| Safari | Yes |
| Edge | Yes |
| Internet Explorer | Yes |
| Opera | Yes |
| Internet Explorer | No |

## Conclusion

In the world of web development, creating captivating web experiences remains a top priority. At the heart of this endeavor lies the art of image styling with CSS, a crucial skill for designers looking to craft visually engaging web projects. In this guide, we have explored three essential CSS properties: aspect ratio, object fit, and object position, that empower developers to take their image styling to the next level.

The concept of aspect ratio, a relatively recent addition to CSS, allows designers to define the width-to-height ratio of images, ensuring that they adapt seamlessly to varying viewport sizes. This property provides a powerful tool for responsive design, enhancing the overall user experience.

Object-fit, on the other hand, offers precise control over how images behave within their content boxes. Whether you need to stretch, scale, or maintain aspect ratios, object-fit provides the means to achieve your desired visual effect.

To complement object-fit, the object-position property allows designers to precisely align images within their containers, adding a layer of customization that can greatly enhance the aesthetics of a website.

## References

1. [CSS Tricks](https://css-tricks.com/)
    
2. [Mozilla Developer](https://developer.mozilla.org/)
    
3. [w3schools](https://www.w3schools.com/css/)