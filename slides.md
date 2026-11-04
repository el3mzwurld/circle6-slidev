---
theme: default
background: "./assets/purple.jfif"
title: Circle 6's Summary of Month 1
info: |
  ## Circle 6's month 1 assessment : In this presentation we take on a summary of what we learnt collectively in our first month at AltSchool Africa

# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 35min
ease: ease-in
overflowY: auto
---

# This is Circle 6

Our Summary of our Month 1 Learnings at AltSchool Africa

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10 c">
  Meet the Circle <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

---
layout: center

---

# An Introduction to Software Engineering

<p class="text-sm mt-4">
Presented by <b>Waheed Oladunjoye</b> and <b>Oyebode Treasure Amaka</b>
</p>

<footer class="mt-20 text-sm">
Authored by : <!--Input authors here-->

</footer>
<!-- Intro : Software Engineering, importance, Algorithms, problem solving, intro to web development -->

---
layout: center

---

## What is Software Engineering?

<div class="text-sm">

<p v-click>
Software engineering is the branch of computer science that deals with designing, building, testing and maintaining software. Coding is only one part. The bigger part is solving the right problem in a way others can understand and maintain.
</p>

<p v-click class="mt-4">
Anyone can write a program that works once on their laptop. Engineering is making it work reliably, for many users, over years. It's the difference between cooking at home and running a restaurant.
</p>

</div>

---

## Types and Why It Matters

<div class="text-sm">

<v-clicks>

* **Web and apps:** front-end, back-end, full-stack and mobile engineers
* **Systems:** embedded, DevOps and security engineers
* **Data and quality:** data engineers, scientists and test engineers

</v-clicks>

<p v-click class="mt-4">
It matters because it drives innovation, keeps software safe and reliable, automates work, connects people, and lets businesses grow.
</p>

</div>

---

## Problem Solving and Algorithms

<div class="text-sm">

<p v-click>
Before writing code, ask: <b>what exactly is the problem?</b> Understand it, break it into small pieces, plan the steps, then test and improve.
</p>

<p v-click class="mt-4">
An <b>algorithm</b> is a step-by-step set of instructions for solving a problem, like a recipe for a computer: <b>Input</b> → <b>Steps</b> → <b>Output</b>.
</p>

<p v-click class="mt-4">
A good one is clear, finishes, gives the right answer every time, and doesn't waste time or memory.
</p>

</div>

---

## Types of Algorithms

<div class="text-sm">

<v-clicks>

* **Searching:** finding a contact on your phone
* **Sorting:** arranging products by price on Jumia
* **Routing:** Google Maps finding the shortest route
* **Text:** spell-check and Google search
* **Math:** a bank app working out interest

</v-clicks>

</div>

---

## Measuring It: Big-O

<div class="text-sm">

Big-O tells us how an algorithm's time and memory use grow as the data grows.

<v-clicks>

* **O(1), very fast:** picking up the top book on a table
* **O(n), normal:** checking every student in a class one by one
* **O(n²), slow:** comparing every student to every other student

</v-clicks>

</div>

---

## The Software Development Life Cycle (SDLC)

<div class="text-sm">

**Understand** → **Design** → **Build** → **Test** → **Deploy** → **Maintain**

<p v-click class="mt-4">
It's a loop, not a straight line. Software is never really finished.
</p>

</div>

---

## Habits Worth Building Early

<div class="text-sm">

* Break big problems into small ones
* Write code others can read
* Use Git from day one
* Test your work
* Keep learning, because tools change but fundamentals don't

<p v-click class="mt-4">
Software engineering isn't about knowing everything. It's about solving problems carefully, one small step at a time.
</p>

</div>

---
layout: center

---

# How the web works

<!-- Introduction to html : CSS and JS mentioned, but not emphasized -->
<div v-click class="text-center">
<p>An Introduction to HTML</p>

<p class = "mt-15">
Authored by : Bethel Amadi.</p>
</div>
---

# HTML: The Structure of a Webpage

<div class="text-sm leading-7">

HTML (HyperText Markup Language) is the standard language used to create and structure webpage content. It organizes headings, paragraphs, links, images, audio, and video so browsers can display them.

<p v-click class="mt-4">
Think of a webpage as a house: HTML provides the rooms and walls, CSS adds the colours and layout, and JavaScript adds actions and interaction.
</p>

```html
<h1>Welcome to My Website</h1>
<p>This is my first webpage.</p>
```

<p v-click>
The <code>&lt;h1&gt;</code> element displays a main heading, while <code>&lt;p&gt;</code> displays a paragraph.
</p>

</div>

---

## Tags and Elements

<div class="text-sm leading-7">

HTML tags are keywords inside angle brackets that tell the browser how to structure content. An element usually has three parts:

<ul class="list-disc list-inside text-left mx-auto max-w-xl">
  <li><strong>Opening tag:</strong> marks where the element begins</li>
  <li><strong>Content:</strong> the information displayed on the page</li>
  <li><strong>Closing tag:</strong> marks where it ends; it includes a slash</li>
</ul>

```html
<p>This is an HTML paragraph.</p>
```

<p v-click class="mt-4">
Here, <code>&lt;p&gt;</code> is the opening tag, the sentence is the content, and <code>&lt;/p&gt;</code> is the closing tag. Together, they form a paragraph element.
</p>

</div>

---

## Attributes: Name and Value

<div class="text-sm leading-7">

Attributes add information or functionality to an element. They are written in the opening tag, usually as a name followed by a value.

```html
<a href="https://www.google.com">Visit Google</a>
<img src="image.jpg" alt="A beautiful landscape">
```

<ul class="list-disc list-inside text-left mx-auto max-w-xl">
  <li>In the link, <code>href</code> is the attribute name and the URL is its value; the text is what visitors see.</li>
  <li>In the image, <code>src</code> gives the image location and <code>alt</code> describes it.</li>
</ul>

</div>

---

## Nested and Void Elements

<div class="text-sm leading-7">

Nested elements sit inside other elements to create a logical content hierarchy. The outer element is the <strong>parent</strong>; elements inside it are <strong>children</strong>.

```html
<div>
  <h2>About Us</h2>
  <p>Welcome to our website.</p>
</div>
```

<p v-click>
The <code>div</code> is the parent; the heading and paragraph are its children. Close nested elements in the reverse order they were opened.
</p>

<p v-click class="mt-3">
Void elements have no content and do not use closing tags. They cannot contain other elements.
</p>

```html
<img src="photo.jpg" alt="My photograph">
<br>
<hr>
<input type="text">
```

</div>

---

## Basic HTML Document Structure

<div class="text-sm leading-7">

The document follows a standard arrangement so the browser can interpret its metadata and page content.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Website</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is my first HTML document.</p>
  </body>
</html>
```

<ul class="list-disc list-inside text-left text-xs mx-auto max-w-2xl">
  <li><code>&lt;!DOCTYPE html&gt;</code> declares an HTML5 document; <code>&lt;html&gt;</code> contains the whole page.</li>
  <li><code>&lt;head&gt;</code> holds metadata: character encoding, the viewport setting for different screen sizes, and the browser-tab title.</li>
  <li><code>&lt;body&gt;</code> holds the visible page content. The <code>lang</code> attribute identifies the page language.</li>
</ul>

</div>

---

## Images: `img`, `src`, and `alt`

<div class="text-sm leading-7">

The <code>&lt;img&gt;</code> element displays an image. Its <code>src</code> attribute gives the file path; <code>alt</code> provides a text alternative if the image cannot load and for screen-reader users.

```html
<img
  src="nature.jpg"
  alt="A beautiful green forest"
  width="500"
  height="300"
>
```

<p v-click class="mt-4">
The optional <code>width</code> and <code>height</code> attributes set image dimensions. Write meaningful, concise alt text for informative images; use <code>alt=""</code> when an image is purely decorative.
</p>

</div>

---

## Audio: Embedding Sound

<div class="text-sm leading-7">

The <code>&lt;audio&gt;</code> element embeds music, recordings, and other sound files. A nested <code>&lt;source&gt;</code> identifies the file and its format.

```html
<audio controls>
  <source src="music.mp3" type="audio/mpeg">
  Your browser does not support audio playback.
</audio>
```

<ul class="list-disc list-inside text-left mx-auto max-w-xl">
  <li><code>controls</code> displays play, pause, and volume controls for listeners.</li>
  <li><code>src</code> gives the media location; <code>type</code> tells the browser its format.</li>
  <li>The text inside the element is fallback content for browsers that do not support audio.</li>
</ul>

<p v-click class="text-sm">Other useful audio attributes include <code>loop</code> (repeat playback), <code>muted</code> (start silent), and <code>preload</code> (hint how to load the file).</p>

</div>

---

## Video: Sources, Posters, and Captions

<div class="text-sm leading-7">

The <code>&lt;video&gt;</code> element plays video in the browser. <code>controls</code> gives viewers playback controls, and <code>&lt;source&gt;</code> specifies the file and format.

```html
<video controls width="600" poster="thumbnail.jpg">
  <source src="tutorial.mp4" type="video/mp4">
  <track
    src="captions.vtt"
    kind="captions"
    srclang="en"
    label="English"
    default
  >
  Your browser does not support video playback.
</video>
```

<ul class="list-disc list-inside text-left mx-auto max-w-xl">
  <li><code>poster</code> shows a preview image before playback starts.</li>
  <li><code>&lt;track&gt;</code> adds timed text; its <code>src</code> points to the caption file, <code>kind</code> sets its type, and <code>srclang</code> and <code>label</code> identify its language.</li>
  <li>Captions include dialogue and relevant sounds; subtitles usually provide dialogue or its translation. Both can help viewers follow the video.</li>
</ul>

</div>

---

## From HTML Structure to JavaScript Behavior

<div class="text-sm leading-7">

HTML gives content its structure. CSS controls how that content looks and is arranged. JavaScript makes the page respond to actions and change over time.

<p v-click class="mt-4">
Now that we have seen how HTML describes a webpage, let's move from its structure to the behavior that makes it interactive.
</p>

</div>

---

layout: center

---

# What is HTML?

<p v-click class ="text-sm">
HTML (or Hypertext Markup Language) is the standard markup language for creating and structuring content on the web. It's one of the pillars for applications built on the web and it is used to create elements such as headers, footers, paragraphs, tables, forms, etc.
</p>

<p v-click class="text-sm mt-[10px]">
Is it a programming language? No. That's because it actually doesn't perform locical computations or execute programming instructions. Instead it can structure and manipulate web pages by using tags, elements and attributes telling web browsers what content should be displayed and how to organize it.</p>
---

## Layout of a traditional HTML Document

```html
<DOCTYPE html> <!--Tell the browser..."this is a html document and it uses hmtl 5"-->

  <html lang="en">
    <head>
      <!-- information about the web page lives inside here...things such as the meta data, title, linked style sheets and scripts, linked fonts etc. -->
    </head>

    <body>
      <!-- this is what the browser renders, elements go in here for example...-->

       <p>This is my first web page.</p>
    </body>
  </html> <!--This is an html tag, everything concerning the html document lives inside this tag-->
```

---

# HTML Tags and Elements

<div v-click class="text-sm">
Tags and elements are the building blocks of html elements, especially in the body. They allow the proper structuring of a web page and it's content. Elements are made up of tags and their content which goes inside the tag, some which may have opening and closing tags, others may just have one tag which self closes.
<br>
For example, navigation bars could go in the <span class="text-red">header</span> tag, or if you wanted to put it in a sidebar you could use the <span class="text-red">aside</span> tag..I like to think of html as a base language, and it can do very good things for you when you can use it simply...but when you can make use of semantic html, it's way more powerful because it can simplify tricky page structures and designs.

<p class="text-sm mt-10">
HTML elements can also have attributes, some which describe them, others allow them to reference files, links or values even. These can help and also impact the way elements behave</p>

```html
<h2 class="header-2">This is a header element</h2> <!--This is an element, with it's h2 tag and it's content(which can be empty) and it's class attribute-->
```

<p class="text-sm">
HTML on it's own is a powerful tool..It's able to perform and simplify tedious tasks on the web by using some nifty elements but HTML on it's own isn't complete. So let's take a look at the pillars of web development that complete web development aside HTML.</p>
</div>

---

## CSS and Javascript

<p v-click>
HTML, CSS and Javascript are the three fundamentals used to create modern web applications. Each of them have a different responsibility but they come together to produce powerful, attractive and interactive digital experiences for users. So what does each do?

<div class="text-sm mt-3.5">
 <ul class="flex flex-col gap-1.5">
 <li>
 HTML provides structure by defining what exists on the page and how it's organized. For example, you can use html to create a login form with fields for name, address, delivery options etc. But by itself HTML does not provide styling or advanced interactive behavior to make that form look good, or submit.</li>

  <li>
 Cascading style sheets allows us to use simple and sophisticated styling to beautify our web pages. It determines colors, spacing, fonts, borders, backgrounds, animations, positioning, responsive layouts etc. CSS can transform our basic form from before into a polished visual interface. It heavily impacts web development and usage of web applications by transforming the user experience between different screen sizes or devices. Snappy animations, beautiful transitions etc. all play a role in making the overall feel of a web page more than just words and images.</li>

 <li>
 The feel we said CSS brings to a web page? Javascript dials that up by adding behaviour and interactivity. It allows the web page to come alive...literally. It makes web applications functional and dynamic, it can execute logic, process data and respond to user actions on the web page. For example, when the user wants to submit our form from before, Javascript can validate, collate results into an object and also send HTTP requests over the web to APIs and databases. It is an extremely powerful pillar that takes web pages from static documents to dynamic tools that run the web.
 </li>
 </ul>
</div>
</p>
---
layout: center

---

# Let's talk about Javascript

<footer v-click class="mt-20 text-sm">
Authored by : Elemi Samuel and Blessing Dawodu.
</footer>
---
layout: center

---

<h1>
What is Javascript?
</h1>

<div v-click class="mt-5">
Javascript is a fundamental building block for web-powered applications. It is the backbone for webpages, and serves as the main provider of application functionality that makes web apps usable, interactive, reliable and intuitive.
</div>

---

## JavaScript and the web

<div class="text-sm">
HTML gives the web page structure and CSS allows styling. Javascript(also referred to as JS) delivers interactivity, it translates problem solving logic and it serves functional behavior to the web page--allowing sites to move beyond static text or designs and respond to user actions as they happen. Let's look at a brief example of what it looks like, then we can start on the javascript basics.

```js
// brief example of javascript code
console.log('This is Elemi Samuel Speaking...')

const color = 'blue'
```

</div>

---

## Variables in Javascript

<p class="text-[14px]">
A variable is a container used for storing data. Think of your RAM as a kitchen, various dishes need cooking and there are various ingridients present within said kitchen all at the same time...well, your variable in this analogy would be a container used to house said ingridient and is saved within the kitchen (memory) so it can be used within a certain context. In javascript, these variables need to be <em>declared</em> in order to be able to house data inside them...and to do this you can either use the <span class="text-purple my-[5px]">let</span>, <span class="text-purple my-[5px]">const</span> or  <span class="text-purple my-[5px]">var</span> keywords to declare a variable.</p>

---

## Naming Variables

<div class="text-sm">

Javascript also has a couple of rules guiding variable names that we have to follow. They are :

* the first character must be a digit
* reserved words or keywords cannot be used as variable names
* if it contains multiple words, use **Camel case**
* if possible use variable specific names, prefferably ones that describe what the specific variable will be housing, also stay away from easily reusable names such as single letters(a, b ,c) or short alphanumeric names(a1, a3, z5)
* you can separate multiple words using the underscore(_), but camelCasing should be the first naming convention at hand.

```js {monaco-run}{autorun: false}
let name  //This is how to declare a variable
name = "Theresa" //Variable definition...This tells Javascript to put "Theresa" inside of the container 'name'
// console.log(name) 
var age = 18 //you can also declare and define in the same line, telling js to make a container 'age' and put "18" in that container all at once
console.log(age)

```
<!-- The nitty gritty : Most programming languages actually treat variables as references to a memory address, whether that's as a pointer or as a direct reference to it's memory address. So yes, you can think of a variable as a container, but under the hood the container itself is a slot in memory, the variable itself is just a reference to it...so when you call a variable, remember you're only referencing a memory address which contains the data you're storing. -->
</div>

---

<div class= "text-sm flex flex-col gap-5">
<h3>Variable use : <span class="text-cyan">const</span></h3>

* Variables declared with const are **constant** values and for that reason, their value cannot be altered after definition.
* For values that could change, it's best practice not to use const.

<h3 class = "text-sm">Variable use : <span class="text-cyan">let</span> and <span class="text-cyan">var</span></h3>

* As opposed to <span class="text-purple-400">const</span>, variables defined using <span class="text-purple-400">let</span> and  <span class="text-purple-400">var</span> allow reassignment of values.

```js{monaco-run}{autorun:false}
const sam = "Elemi Samuel"
console.log(sam)
// sam = "Munachi" //This won't work because sam has already been assigned a value as a constant variable. 

let name = "Oluwasetemi"
console.log(name)
name = "Munachi"
console.log(name) //name changed and "Munachi" prints
```

</div>
---

# Data Types

<p v-click>
A value in JS has to be of a certain data type. The data type defines the operations a variable can do and also what methods can act upon it
</p>
<div v-click class = "text-sm">

<span class = "text-red-400">Number</span>

* A number in javascript can be an integer or a floating point, both fall under the <span class = "text-red-400">Number</span>
 umbrella.

```js{monaco-run}{autorun: true}
const age = 20 //integer
const floatingPoint = 14.458 //floating point
console.log(typeof floatingPoint)
console.log(typeof age)
```

</div>

---

# Data Types (cot'd)

<div v-click class = "text-sm">

* A <span class = "text-red-400">String</span> must be surrounded by air quotes, that could be back ticks, single or double quotes.

```js{monaco-run}{autorun: true}
const myName = "Elemi Samuel" // ✅ good practice
const myName2 = `Elemi Samuel` // ✅ good practice
const name  = "Elemz' // ❌ bad practice
//in summary, ensure you stay consistent in what quotes you use to open and close a string
```

* The <span class = "text-red-400">Boolean</span> type only consists of two possible values...true and false.

```js{monaco-run}{autorun: true}
const bool = true
const isEligible = false
```

</div>

---

## Data Types (continued)

<div v-click class = "text-sm">

* An <span class = "text-red-400">Object</span> type is a collection of keys and values used to store collections of data.

```js{monaco-run}{autorun: true}
const person = {name : "Ebere", age : 25, degree: true, school : "SOE"}
```

* The <span class = "text-red-400">undefined</span> type is reserved for variables that have not been assigned a value
* The <span class = "text-red-400">null</span> type is a special value that represents an empty variable.

</div>

---

There's actually an unresolved flaw in Javascript dating back years

<div v-click class="text-sm">

* The <span class = "text-red-400">null</span> type actually returns an object type.

```js{monaco-run}{autorun: true}
const name = null
console.log(typeof name)
```

<p>It originates from how data types were stored in the first place, with the object and null types sharing type tags that were slightly similar and hence misclassified by the typeof operator.</p>
</div>

<p v-click class="text-sm">Can this be resolved? of course. But it would break many legacy websites and libraries that rely on this tiny hiccup...so it remains the flaw of Javascript that has grown to be beautiful I guess 🤷🏽‍♂️ </p>
---

# Collaboration Practices within Software Development

<!-- git and version control with GitHub -->
