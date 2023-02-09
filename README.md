# Frontend Mentor - Skilled e-learning landing page solution

This is a solution to the Skilled e-learning landing page challenge on [Frontend Mentor](https://www.frontendmentor.io/).

## Table of contents

- [Overview](#overview)
	- [Screenshot](#screenshot)
	- [Links](#links)
- [My process](#my-process)
	- [Built with](#built-with)
	- [What I learned](#what-i-learned)
	- [Continued development](#continued-development)
	- [Questions to community](#questions-to-community)
- [Author](#author)

## Overview

### Screenshot

![](./Screenshot.png)

### Links

- Solution URL: [GitHub - OignonFugace/FEM__skilled-elearning-landing-page](https://github.com/OignonFugace/FEM__skilled-elearning-landing-page)
- Live Site URL: [Frontend Mentor | Skilled e-learning landing page](https://oignonfugace.github.io/FEM__skilled-elearning-landing-page/)

## My process

### Built with
Vanilla HTML & CSS. 


### What I learned
- About custom properties
	- This was the first time that I tried to leverage the capabilities of CSS custom properties together with media queries. 
	- This was the first time I used custom properties to define globally font related properties. 
	- For each course card I used an inline style for defining the path to the svg icon via a custom property that I can then access in the CSS in the element in which it was defined. I wanted first to use the `attr()` CSS function but I read that it is not possible to access an attribute this way inside a `url()`. Reference : [The CSS attr() function got nothin' on custom properties | CSS-Tricks - CSS-Tricks](https://css-tricks.com/css-attr-function-got-nothin-custom-properties/)
- I had the chance to practice CSS Grid layout system, both for the courses cards section and for the cards themselves (keeping the "Get Started" buttons at the bottom of each card in a consistent fashion).  
- I used the `<picture>` element.
- I struggled positioning the hero image of tablet and mobile devices. It would have been easier setting them as a background image, but I thought that as those images carry some information they should be in the markup. Hence I absolutely positioned them inside their grid cell and used `top` and `left` and `tranform: scale()` to place them where I wanted. 
- I used this one liner for responsive padding (reference: [Using max() for an inner-element max-width | CSS-Tricks - CSS-Tricks](https://css-tricks.com/using-max-for-an-inner-element-max-width/)): 
```css
.content-wrapper {
	padding: 0 max(max(1rem, 4%), 50% - var(--contentWidth) / 2);
}
```


### Questions to community
- Was there a more straightforward way of positioning hero images while keeping them in the markup ? 
- In the design, it seems that the background gradient doesn't start at the top but is offset to the start of the course cards section. How can I achieve that result? 


### Continued development
- I discovered that it is not possible to transition gradients (the buttons in this particular challenge) : [Transitioning Gradients | CSS-Tricks - CSS-Tricks](https://css-tricks.com/transitioning-gradients/). I'll dive in the different techniques to overcome that latter. This could also help : [hover - CSS background (gradient) transition not working - Stack Overflow](https://stackoverflow.com/questions/17952468/css-background-gradient-transition-not-working). 
- I really need to dive deeper in gradients, which I didn't do this time. 
- Any other feedback is greatly appreciated!


## Author
- Website - [Oignon Fugace - par Tanguy Freycon](https://oignonfugace.com/)
- Frontend Mentor - [@OignonFugace](https://www.frontendmentor.io/profile/OignonFugace)
