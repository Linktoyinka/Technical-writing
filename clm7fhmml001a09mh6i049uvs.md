---
title: "Choosing Between “display: none” and “visibility: hidden” in CSS: A Practical Guide"
datePublished: Wed Sep 06 2023 07:38:57 GMT+0000 (Coordinated Universal Time)
cuid: clm7fhmml001a09mh6i049uvs
slug: choosing-between-display-none-and-visibility-hidden-in-css-a-practical-guide
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1693985860069/d2d0d41e-7623-42f3-b29a-c03c8dd2263e.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1693985876226/6d240403-2656-4efc-8659-80496bef9762.jpeg
tags: css, html5, beginners, frontend-development

---

There are various reasons why items on the frontend of websites need to be hidden; using "display: none" or "visibility: hidden" accomplishes this for us. Their impact on website accessibility and design is what sets them apart. To further understand how the two options impact your websites, we will study them in this article.

## Introduction

HTML is the markup language that makes up the body of web pages, while CSS is mainly used to make websites look good. One of the most common things developers do is show and hide HTML components, and there are a few different ways to do it. Two of the most common ways to hide and show HTML are `display: none` and `visible: hidden`, while how to use them is confusing. This article will address how these two methods work and when to use them with practical examples to help you understand.

## Prerequisites

1. Basic understanding of the markup language (HTML)
    
2. Good background knowledge of CSS
    
3. Familiarity with IDE
    

## CSS Rule

This is a collection of selectors and declarations found in CSS code. These rules are used to beautify HTML components and are also in charge of hiding elements from users' view. Two of the rules for hiding items are "display: none" and "visibility: hidden".

![CSS syntax](https://puzzleweb.ru/en/images/css/1_1.png align="center")

### The “display: none”

One of the most popular and effective CSS properties is `display`, which is well known with values such as flex and grid. It is one of the CSS properties used to conceal front-end components. The display property's default value is `block`.

When it comes to hiding elements, this is the most popular method. If a value of none is added to the property, the element will be made invisible so that users won't see it on the website. The default value is block.

### How to use “display: none”

To use this property, select the element you want to hide with the suitable selector, either tag, class, or ID. Then, add the property and its value to it.

```css
div { display: none;}
/** to hide element **/
```

To unhide your element, change the value of the property to its default value.

```css
div { display: block;}
/** to unhide element **/
```

### When to use “display: none”

This property has several use cases. Some of these are;

1. **Hiding Elements Responsively:** Web developers often use 'display: none' to hide elements on smaller screens or devices to create responsive designs. For example, you might want to hide a large sidebar navigation menu on mobile devices to save screen space.
    
    ```css
    @media (max-width: 768px) {
       .sidebar {
         display: none;
       }
    }
    ```
    
2. **Conditional Rendering**: You can use 'display: none' to conditionally show or hide elements based on user interactions or specific conditions in your web application. This is common in dropdown menus, tooltips, or modals.
    
    ```css
    .hidden {
      display: none;
    }
    ```
    
3. **Preventing Content from Being Printed:** You might want to hide certain elements (like navigation menus, advertisements, or buttons) when developing a web page for printing because they wouldn't make sense on a printed document.
    
    ```css
    @media print {
      .print-hide {
        display: none;
      }
    }
    ```
    
4. **Accessibility and SEO:** In some cases, you might have content that you want search engines or screen readers to be able to view but not regular users. You may ensure that the material is still contained within the HTML structure but is not shown on the page by using the display: none style.
    

### Practical example

%[https://codepen.io/linktoyinka/pen/abPBEee] 

It's important to note that 'display: none' completely removes an element from the document flow, which can affect layout and accessibility. Developers should use it sparingly, considering its impact on user experience and the specific requirements of their projects.

### The Visibility Property

The visibility property is another widely used method to hide elements. To use this property, the value "hidden" will be assigned to it to make it invisible to users. The default value is visible. The difference between this property and "display: none" is that when you use "display: none," the element is completely hidden from users' view, whereas "visibility: hidden" hides the element from users' view but leaves a blank space where the element would have been.

### How to use “visibility: none”

Choose the element you want to hide using the appropriate selector, such as a tag, class, or ID, to use this property. Add the property and its value after that.

```css
div { visibility: hidden;}
/** to hide element **/
```

To show your element, change the value of the property to its default value.

```css
div { visibility: visible;}
/** to unhide element **/
```

### When to use “visibility: hidden”

This attribute is typically used when you want to keep your current layout unaffected while trying to hide an element until an action is made. Consider the form for a moment. If the user enters incorrect information or leaves a field empty, you might want to show an error message when working on a form. The area is already in the layout with "visibility: hidden"; all that is needed is a trigger action to make the content visible. However, if you set "display: none" to an element, it will reappear with its space, which will cause the other components to move and change the existing layout.

### Practical example

%[https://codepen.io/linktoyinka/pen/ZEVBrRz] 

Remember that even though an element is visibly hidden by the property "visibility: hidden," it still occupies space in the layout. It's critical to select a suitable CSS property (such as "display: none" or "visibility: hidden") based on the needs of your design.

## Conclusion

In conclusion, knowing when to use the CSS properties "display: none" and "visibility: hidden" is crucial for efficient web development. Use the option "Display: none" to completely remove an element from the layout and make it invisible. It is appropriate for situations requiring immediate removal and responsive design. However, because of the potential effects on layout and accessibility, it should only be used sparingly.

On the other hand, 'Visibility: hidden' conceals an element while maintaining its layout space. When you want to keep the layout stable and reveal elements in response to certain user actions, it's useful. For form error messages, this property is especially helpful.

Which of these CSS characteristics you should utilize ultimately depends on the precise requirements of your project. Making the finest decisions, which enhance user interactions and maximize layouts, requires developers and designers to be aware of these distinctions. CSS competency requires both an understanding of the properties and judicious application of those features to create excellent online experiences.

## References

1. [W3 School](https://www.w3schools.com/cssref/pr_class_display.php)
    
2. [PuzzleWeb](https://puzzleweb.ru/en/css/1_css_syntax.php)