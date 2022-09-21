# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See active states for interactive elements

### Screenshots

![](/design/solution-desktop.png)
![](/design/solution-mobile-active.png)

### Links

- Live Site URL: [https://neon-sprite-1f6015.netlify.app/](https://neon-sprite-1f6015.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I practiced using @media screens with this excercise and experimented with the best ways to define widths and heights for different-sized screens. At first, I tried using percentages to define the sizes, but it didn't work nicely with placing the image and information card next to each other. In the end, I defined the sizes using pixels.

The screen sizes also led me to figure out how to switch out images based on the screen layout. First, I used a simple CSS property/value pair - `display: none` to hide the image I didn't need. However, after receiving feedback regarding proper semantic use of the HTML `<picture>` tag and SEO best practices, I updated my code to swap the images in the HTML file rather than using CSS.

To see how you can add code snippets, see below:

```html
<picture>
  <source media="(max-width:624px)" srcset="images/image-product-mobile.jpg">
  <img src="images/image-product-desktop.jpg" alt="Gabrielle Chanel Perfume Bottle." class="card__image">
</picture>
```
```css
.card__image{
    width: 300px;
    border-radius: 3% 0 0 3%;
    margin-top: 3px;
}
```

### Continued development

This also seems like a good excercise to try CSS grid, or maybe some libraries and frameworks such as React, TailwindCSS, or Bootstrap.

## Author

- Website - [Ticia Francisco](https://ticiafrancisco.netilfy.app/)
- Frontend Mentor - [@hydrx](https://www.frontendmentor.io/profile/hydrx)
- Twitter - [@elephantscode](https://www.twitter.com/elephantscode)
