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

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# An Introduction to Software Engineering

<!-- Intro : Software Engineering, importance, Algorithms, problem solving, intro to web development -->

---
layout: center

---

# How the web works

<!-- Introduction to html : CSS and JS mentioned, but not emphasized -->

---
layout: center

---

# What ties it all together ?

<br>
<v-click>Let's talk about Javascript</v-click>

---
layout: center

---

<h1>
What is Javascript?
</h1>

<div v-click class="mt-5 text-[14px] leading-6">
Javascript is a fundamental building block for web-powered applications. It is the backbone for webpages, and serves as the main provider of application functionality that makes web apps usable, interactive, reliable and intuitive.
<br>
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

<div class="text-sm mt-2.5">
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

<span class = "text-red-400 text-[16px]">Number</span>

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
