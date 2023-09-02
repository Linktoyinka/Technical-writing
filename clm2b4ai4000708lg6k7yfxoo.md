---
title: "CSS Animation Made Extremely Ease"
datePublished: Sat Sep 02 2023 17:37:45 GMT+0000 (Coordinated Universal Time)
cuid: clm2b4ai4000708lg6k7yfxoo
slug: css-animation-made-extremely-ease
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/SXihyA4oEJs/upload/049716baaff45feaf660b66438b32b73.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1693672689108/1643cb6a-fffd-4d4e-ad47-7a870d37e66b.jpeg
tags: css, css-animation, javascript-library, frontend-development

---

Animating in CSS using keyframes requires time and effort. This is because it is hard to achieve in most cases. Let me introduce you to a JavaScript library named Animate on Scroll **(AOS)**. AOS makes animation easy by adding attributes to your HTML tags.

# Introduction

Having a website is a must for anyone who wants to have an online presence. When you have the website, you can tell the people on the internet about what they do or the services they render. The joy of every website owner is for people to find their website interesting. This will make website visitors spend more time and read more content on your website.

One of the ways to do this is to add friendly animations to your website and not overuse them. Most developers don't animate websites because it takes time and is stressful. With Animate on Scroll, animating websites is now easier than before. In this article, I will teach you how to animate your website with **AOS**.

# **Prerequisites**

* Basic knowledge of HTML and CSS.
    
* Familiarity with JavaScript and JavaScript concepts like object.
    
* Familiarity with integrated development environment (IDE) and terminal/command line for running code.
    

# Animate on Scroll (AOS)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1693655675355/d6209907-7d9a-4bf6-b014-b51c264b5c88.jpeg align="center")

**AOS** is a JavaScript library with over 20 predefined animations for your websites. To add these animations to your website, you will need to install the library on your website.

## Installation

There are two ways of installing **AOS**:

1. **Basic Installation:** Install the library by adding an external stylesheet to your `head` tag.
    
    ```xml
      <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
    ```
    
    Add script right before the close of `</body>` tag and initialize **AOS**.
    
    ```xml
      <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
      <script>
        AOS.init();
      </script>
    ```
    
2. **Package Managers:** Install the package using yarn `yarn add aos@next` or npm `npm install --save aos@next` After that, import the script and styles and initialize **AOS**.
    
    ```javascript
    import AOS from 'aos';
    import 'aos/dist/aos.css'; // You can also use <link> for styles
    // ..
    AOS.init();
    ```
    

## How to use it

### **Basic usage**

Adding the animation to your HTML content is simple. To do this, you will add the `data-aos` attribute for the effect on your HTML.

```xml
<div data-aos="fade-in"></div>
```

Also, you can use the **AOS** attributes in all HTML tags.

A few of the predefined **AOS** animations are put into use below:

%[https://codepen.io/linktoyinka/pen/JjwKgLo] 

You can check the remaining available animations on the [AOS website](https://michalsnik.github.io/aos/).

### Advance usage

Adding **AOS** animations to your website with settings you would like to set yourself, like duration, delay, and offset. You can do this by adding the attribute you want to edit to the AOS default attribute `data-aos-*`.

```xml
  <div
    data-aos="fade-up"
    data-aos-offset="200"
    data-aos-delay="50"
    data-aos-duration="1000"
    data-aos-easing="ease-in-out"
    data-aos-mirror="true"
    data-aos-once="false"
    data-aos-anchor-placement="top-center">
  </div>
```

A few of the predefined advanced usage of AOS animations are put into use below:

%[https://codepen.io/linktoyinka/pen/zYyKOGv] 

You can check the remaining available animations in the table below.

| **Attribute** | **Description** | **Example value** | **Default value** |
| --- | --- | --- | --- |
| `data-aos-offset` | Adjust the offset to start the animation sooner or later (px). | 200 | 120 |
| `data-aos-duration` | Animation runtime (ms). | 600 | 400 |
| `data-aos-easing` | Select the timing function for the element easing feature in multiple ways. | ease-in-sine | ease |
| `data-aos-delay` | Animation delay (ms). | 300 | 0 |
| `data-aos-anchor` | Offset value that will be used for the anchor element instead of the default set value. | #selector | null |
| `data-aos-anchor-placement` | Element on the screen that should be in the anchor position to start the animation. | top-center | top-bottom |
| `data-aos-once` | Select whether the animation should play only once or each time you scroll up or down to an element. | true | false |
| `disable` | The condition in which AOS should not function. | mobile | false |

### Global settings

If you are using the same advanced attributes for your animations, setting these attributes one after the other will take more time, and you will also write more lines of code. We will provide a solution to this using this setting.

To do this, add the options object to the `init()` function, like this:

```xml
  <script>
    AOS.init({
      offset: 200,
      duration: 600,
      easing: 'ease-in-sine',
      delay: 100,
    });
  </script>
```

## Make your own animation

We can create new animations with AOS if we don't like the default animations that AOS gives us.

To do this, we will work on two states, which are

1. Before animation
    
2. After animation
    

```css
/* Before animation*/
[data-aos="new-animation"] {
  transform: rotate(300deg) scale(0.3);
  opacity: 0;
  transition-property: transform, opacity;
}
/* After animation */
[data-aos="new-animation"].aos-animate {
  transform: rotate(0) scale(1);
  opacity: 1;
}
```

To use our newly created animation, we will add the attribute `data-aos="new-animation"` to the element we want to animate.

See our newly created animation in action below.

%[https://codepen.io/linktoyinka/pen/RwEGbmq] 

# Conclusion

In this article, we talked about Animate on Scroll (AOS), one of the JavaScript libraries for animation. We break down every detail of how we can use this library to animate our websites. We also talk about how to make our own animations.

We can animate our websites now without worrying about the stress that comes with the default CSS way of animating elements on the front end of our websites.

# References

1. [AOS Website](https://michalsnik.github.io/aos/)
    
2. [AOS GitHub Repository](https://github.com/michalsnik/aos)