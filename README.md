# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./images/screenshot.png)


### Links

- Live Site URL: [https://tender-rosalind-138900.netlify.app/]

## My process

### Built with

- HTML5 and BEM
- CSS + SASS
- Flexbox
- Custom responsive breakpoints

### What I learned

It's been quite difficult to find how to make the black and white picture look purple in CSS, but eventually succeeded with a pseudo-element ::after with a purple filter positionned over the picture. Then the CSS property "mix-blend-mode" does a great job !

```css
.picturecontainer {
  position: relative;
}

.picturecontainer::after {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  content: '';
  background: $color-image_tint;
  mix-blend-mode: multiply;
  border-radius: .8rem .8rem 0 0;
}
```

### Continued development

- I still need to improve with Flexbox, not always comfortable with it
- Also need more practising of responsive design, not sure if the breakpoints I've set are consistent enough

### Useful resources

- [Most common screen resolutions](https://www.designrush.com/trends/website-dimensions) - I have set the common screen resolutions in my browser's adaptive view to find the best settings to make it fully responsive.

## Author

- Frontend Mentor - [@JonathanCazzaro](https://www.frontendmentor.io/profile/JonathanCazzaro)
- Twitter - [@CazzaroJonathan](https://twitter.com/CazzaroJonathan)


