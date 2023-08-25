---
title: "The Essence of JavaScript in Web Development"
datePublished: Tue Aug 22 2023 01:32:57 GMT+0000 (Coordinated Universal Time)
cuid: clllmt62o000409mggwa16xth
slug: the-essence-of-javascript-in-web-development
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692696929201/b0eb9b15-a982-463d-b180-ec3326d1ab29.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1692667899243/539b85cf-7a55-4390-92c7-ed880b2bed92.jpeg
tags: js, javascript, javascript-framework, javascript-library

---

I know you have been wondering what exactly this JavaScript **(JS)** is that has gathered so much attention everywhere. The answer is straightforward: JS is a very potent scripting and programming language that web developers frequently utilize to add distinctive features like interactivity to web pages, applications, servers, and even games. What makes it great is the ability to work on the front-end and the back-end of any software, which most programming languages lack.

JavaScript, on the other end, can’t stand alone. In this regard, to begin your journey in JS, you need a solid understanding of two other standard web technologies, which are HTML and CSS.

* HTML is the skeleton of a website that frames how the website will be structured.
    
* CSS adds style and formatting to the skeleton, making it beautiful.
    
* JavaScript turns those beautified skeletons into something that a user can interact with.
    

![the relationship between HTML, CSS, and JS.](https://cdn.hashnode.com/res/hashnode/image/upload/v1692558951414/7a59078a-3f81-4aef-a99a-70846ba47f81.png align="center")

Brendan Eich created JavaScript in 1995. It was initially created for Netscape 2, and it became the ECMA-262 standard in 1997 after being given to ECMA. The Mozilla Foundation then kept working on creating JavaScript for the Firefox browser.

| Year | ECMA Version |
| --- | --- |
| 1997 | ES1 |
| 1998 | ES2 |
| 1999 | ES3 |
| 2008 | ES4 |
| 2009 | ES5 |
| 2016 | ES6 |

In 2018, the ES6 version was developed to provide full support for all browsers.

The general usage of JavaScript by most web developers is to modify HTML and CSS to update the user interface dynamically. This is usually done by the Document Oriented Model **(DOM)**. You have to note that the written code on your web page is loaded and executed in the order of their arrangement. JS has to come last in the web document to avoid errors when the web page is loaded. This is because the HTML and CSS that are to be modified have to be loaded first before the script can modify them. There are two ways to add JavaScript to a web document:

* **External Linking:** This is the practice of having the script in a separate file named with the extension .js, for example, script.js. The created file will be linked using the script tag with the src attribute right below the closing of the body tag and before the close of the HTML tag.
    
    ![External JS linking](https://cdn.hashnode.com/res/hashnode/image/upload/v1692559203325/5c9f3fae-d006-4818-bd1d-1fc53c5f17df.png align="center")
    
* **Internal Linking:** This is the practice of having the script in the same HTML document using the script tag without the src attribute right below the closing of the body tag and before the close of the HTML tag. The script will go in between the opening and closing of the script tag.
    
    ![ Internal JS linking](https://cdn.hashnode.com/res/hashnode/image/upload/v1692559318682/26b87199-cb89-4ae5-987a-12ed075f674a.png align="center")
    

## **JavaScript Data Types**

All programming languages have structures on which they are built. These structures are accompanied by built-in data types to hold different types of values, and these differ from one language to another. For JavaScript, there are two types of data types into which data types are classified.

1. Primitive data type.
    
2. Non-primitive (reference) data type.
    

**Primitive data type:** In JS, a primitive data type is referred to as an object and has no methods or properties. There are 7 primitive data types:

* **String:** This refers to data that is text and is enclosed with a quotation mark.
    
    ```javascript
    let text = "This is a string";
    // A string that is stored in a variabled identified as text
    ```
    
* **Number:** This refers to data that is numeric or an integer. It does not require being enclosed in a quotation mark.
    
    ```javascript
    let num = 45;
    // A number that is stored in a variable identified as num
    ```
    
* **Boolean:** This represents data that only defines if a variable is true or false.
    
    ```javascript
    const listData = true;
    const bulletData = false;
    // Boolean data defined with true or false
    ```
    
* **BigInt:** This is a type of data that is an integer but in its arbitrary precision format. This is created by adding the suffix **n** to an integer.
    
    ```javascript
    const value = 98345689009876543n;
    // BigInt
    ```
    
* **Undefined:** As the name states, this is a type of data that is not defined. The variable has a variable identifier, but there’s no assignment operator or value.
    
    ```javascript
    let west;
    console.log(west); // undefined
    ```
    
* **Symbol:** An item of the specified data type named a symbol can also be referred to as a symbol value. This is an immutable primitive value. For instance,
    
    ```javascript
    // two symbols with the same description
    const textA = Symbol('hi');
    const textB = Symbol('hi');
    ```
    
    Even though text A and text B both contain the word "hi," they vary because they are of the symbol type.
    
* **Null:** Null is a special value in JavaScript that denotes an empty or undefined value. For instance,
    
    ```javascript
    const number = null;
    ```
    

**Non-Primitive data types:** These data types are the names given to objects in JavaScript. They descend from the primitive data types in JavaScript and are additionally known as derived data types or reference data types. Non-primitive data type variables are kept in the system's heap memory, whereas primitive data type variables are kept in the stack area.

* **Object:** An object in Javascript is a variable that has properties and methods defined for it. Everything is an object in JS.
    
    Let's look at how JavaScript can be used to create an object:
    
    **Creating an object with a constructor:**
    
    ```javascript
    // creating an empty object
    let obj = new Object();
    
    // creating a user-defined object
    let school = new School();
    ```
    
    **Making an object using the literal notation:**
    
    ```javascript
    // creating an empty object
    var cube = {};
    
    // Here length and breadth are keys and
    // 25 and 40 are the values
    var rectangle = {length: 25, breadth: 40};
    ```
    
* **Array:** Using an array, we can group several elements with comparable properties under a single name.
    
    Let's look at how to do it with JavaScript:
    
    ```javascript
    // creating an empty array (no arguments)
    var arr1 = new Array();
    
    // creating an array with the number of elements (a single argument)
    var arr2 = new Array(7);
    
    // creating an array with multiple values (two or more arguments) 
    var arr3 = new Array(4, 6, 8, "string");
    ```
    
* **RegExp:** The RegExp object in JavaScript compares a string to a certain pattern. Using the comparison capabilities of the RegExp object, we can determine whether a regular expression pattern is present in the string or not.
    
    Let's look at how to do this in JavaScript:
    
    **Using a constructor for creating a RegExp:**
    
    ```javascript
    // defining a pattern to compare with a string using
    // the RegExp constructor
    var regex = new RegExp('pattern');
    ```
    
    **Making a RegExp by enclosing the pattern in forward slashes:**
    
    ```javascript
    // defining a pattern with a modifier to compare
    // with a string using forward slashes
    var regex = /pattern/modifier;
    ```
    

## **JavaScript Frameworks**

For quite some time, the development of applications has heavily relied on JavaScript frameworks. This has undeniably marked a milestone for this programming language.

Another noteworthy benefit of JavaScript is its compatibility with JS frameworks. These frameworks are widely utilized to access and leverage pre-existing JavaScript code that caters to functionalities and capabilities.

### **Popular JavaScript front-end frameworks**

**React.JS**

Rather than being a JS framework, React.JS primarily serves as a library. It is also thought to have the fastest growth among JS frameworks, with 1,000 contributors on GitHub.

The elements of this framework may also be created, utilized for various applications, and distributed for use by the general public.

Additionally, it is said to be better suited for sophisticated, complex, high-load software solutions.

**Vue.JS**

Vue, another 2016 release, has proven to be the best of them all since it mixes Ember, React, and Angular into one handy package.

Additionally, it may be proven to be a cure-all for sophisticated single-page apps (SPAs) and effective in any scenario where efficiency is valued above app structure or clear code.

**Angular JS**

Most often, AngularJS is described as an MVW (model-view-whatever) framework that offers several advantages to various start-ups and mid-sized businesses.

It is mostly used for two-way data binding (changes in the back-end are immediately reflected in the UI), rapid code creation, and simple testing of any app component.

After being released, the framework has developed beyond all recognition and is now the most popular JS framework for building single-page applications.

The component-based design, enhanced dependency injection, effective logging service, inter-component connections, and many other features of Angular are also a blessing.

## **JavaScript as a back-end tool**

Back-end development is the term used to describe the server side of web development, where you, the developer, build the code that powers the web application. When a user is exploring the web, they view and interact with the front-end, which is powered by the back-end, which normally operates on a web server.

The following are the responsibilities of the back-end

1. Keeping and getting information out of a database.
    
2. Data processing.
    
3. Data transmission to the front-end
    
4. Getting information from the front-end
    
5. Control of user sessions.
    
6. The application's security.
    

Node.JS, an environment for running JavaScript, enables JavaScript code to be run outside of a web browser. It was released in 2009 so that server-side applications could be run using JavaScript. It is a cross-platform environment based on the V8 JavaScript engine and has a ton of libraries and tools to help developers create reliable apps.

Node.JS is a well-liked back-end development framework since it is quick, lightweight, and effective. Next.JS and Express.JS are two other popular JavaScript frameworks.

### **Popular JavaScript back-end frameworks**

**NodeJS**

A cross-platform, open-source server-side JavaScript run-time environment is Node.js. It can drive asynchronous I/O thanks to its event-driven design. Similar characteristics like packing, threading, and loop formation are present in this architecture.

Features;

* Given that it was created using the V8 JavaScript engine from Google Chrome, the library executes code quickly.
    
* The server doesn't have to wait for any APIs to respond with data because all of them are asynchronous.
    
* Since it is open-source, it has a sizable community and several incredible models to give Node.js apps more functionality.
    

**Next.JS**

Most commonly, Next.js, a straightforward JavaScript framework, is employed on the back end to construct applications utilizing the React framework.

The primary objective of Next.js is to streamline the development of React applications, making the process as uncomplicated as can be.

Features;

* A straightforward structure.
    
* Quick performing.
    
* Easy to understand and utilize.
    

**Express.JS**

Express stands out as one of the finest back-end frameworks for JavaScript scripting. It is the preferred choice for crafting web applications and APIs due to its speed and simplicity.

Its primary role is to serve as the default server framework for Node.js and as a front-end framework for Angular.js.

Features;

* Quick performing.
    
* Simple to learn.
    
* Straightforward and light.
    
* Robust and relatively immune to coding errors; it boasts extensive support for numerous plugins.
    

## Conclusion

Imagine a world without JavaScript - websites would be static, apps would lack that interactive magic, and games would lose their dynamism. JavaScript, my friend, is like a wizard's wand in the digital realm. It's not just a language; it's a key that unlocks a universe of possibilities!

Think about it. Whether you're crafting a stunning web app, diving into the realm of mobile app development, cooking up the next gaming sensation, or even tinkering with a sleek terminal app, JavaScript has got your back. It's the Swiss Army knife of coding languages, armed with an array of tools and frameworks to help you bring your ideas to life.

So, what are you waiting for? Jump into the world of JavaScript, and let your creativity run wild. Who knows what incredible things you'll build? It's time to embark on a coding adventure that knows no bounds!