# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- [Acknowledgments](#acknowledgments)

## Overview

This challenge involved building a straightforward informational card. It threw a curveball: to adjust font size on mobile screens without using media queries.

### The challenge

Users should be able to:
- See hover and focus states for all interactive elements on the page

### Screenshot

![Here's a screenshot of a mobile view of my solution](https://github.com/WeatherheadOnline/FrontEndMentor_Blog-preview-card-/blob/main/project%20screenshot.png)

### Links

- Solution URL: [Here](https://www.frontendmentor.io/solutions/flexbox-spacing-on-a-blog-preview-card--187lTid8R)
- Live Site URL: [https://weatherheadonline.github.io/FrontEndMentor_Blog-preview-card-/](https://weatherheadonline.github.io/FrontEndMentor_Blog-preview-card-/)

## My process

I started by visually breaking the page into separate elements and creating html elements for each. Next I used the design file to determine colors, fonts and font sizing, and some beginnings of dimensions and spacing. To fine-tune the vertical spacing of the elements on the card, I removed margins on each element, grouped two nested flex boxes, and used the `gap` property to specify spacing.

I initially had some trouble getting the image to look consistent on a range of smartphone and tablet screens. The image's width was set to 100% of the container width, and I was controlling the height based on the image's representation in the design file. However, variety of card element widths on mobile devices precluded using `min()` or `max()` to set the image height. Since I needed distinctly different aspect ratios for desktop vs mobile, I ended up using a media query.

Decreasing the font size on mobile without using media queries was challenging. I researched how others had approached the problem. Consequently I researched `clamp()`, although I eventually used `min()`.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

This challenge taught me about the `clamp()` function, and to be open to using alternatives to media queries. I also gained valuable experience in creating consistent results across different screen sizes and types, using a combination of `min()` / `max()`, `rem` units, and viewport width units.

### Continued development

I am now aware of the `clamp()` function but not at all familiar with its use, so I'd like to find ways to get more experience utilizing it. I'd also like to continue looking for more elegant solutions to the problem of setting the image to the desired aspect ratio without using a media query.

### Useful resources

- [CSS min(), max(), and clamp](https://web.dev/articles/min-max-clamp#:~:text=Note%3A%20When%20using%20a%20calculation,how%20to%20use%20these%20functions.) - This article was a helpful starting point in learning about how to use the `clamp()` function.
- [How does clamp() differ from setting width, max-width, & min-width?](https://stackoverflow.com/questions/70157949/how-does-clamp-differ-from-setting-width-max-width-min-width) - The top answer to this stackoverflow question helped me understand how `clamp()` works.
- [@devdrivenai's solution](https://www.frontendmentor.io/profile/devdrivenai) helped explain how to approach the font-size problem and directed me towards the first link listed above (along with other resources).

## Author

- Website - [www.weatherheadonline.com](www.WeatherheadOnline.com)
- Frontend Mentor - [@WeatherheadOnline](https://www.frontendmentor.io/profile/WeatherheadOnline)
- LinkedIn - [@eddieweatherhead](https://www.linkedin.com/in/eddieweatherhead/)


## Acknowledgments

Huge thanks to @devdrivenai for providing detailed documentation and resources in their solution to help others on this challenge.