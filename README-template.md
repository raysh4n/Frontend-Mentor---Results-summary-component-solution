# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- **Bonus**: Use the local JSON data to dynamically populate the content

### Screenshot

Desktop
![](./Screenshot%202025-01-10%20at%2017-09-58%20Frontend%20Mentor%20Results%20summary%20component%20desktop.png)

Mobile: 
![](./Screenshot%202025-01-10%20at%2017-10-41%20Frontend%20Mentor%20Results%20summary%20component%20mobile.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

- using aspect ratio. make sure either the width or height is specified. aspect ratio 1/1 means -> since width already set to 12rem, height will be the 12rem too since 1:1 ratio.

```css
.circle {
	width: 12rem;
	aspect-ratio: 1/1;  /*THIS*/
	background-image: linear-gradient(
		var(--clr-violet-blue),
		var(--clr-persian-blue)
	);
	border-radius: 50%;
	display:flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	gap:0.5rem;
	margin-inline: auto;
}
```

- Variable is just a place to hold value. It can be like this 
```css
	--clr-light-red: 0, 100%, 67%;
```

- Variable applied not only at :root, but can be at other classes as well, which can be used as a placeholder first. 

```css

.summary__wrapper {
	display:flex;
	justify-content: space-between;
	padding:1rem;
	border-radius: 10px;
	background-color:hsla(var(--item-color),0.151);
}

.summary__criteria {
	color:hsl(var(--item-color));
}


.summary__wrapper--red {
--item-color:var(--clr-light-red);
}


.summary__wrapper--yellow {
--item-color:var(--clr-orangey-yellow);
}


.summary__wrapper--green {
--item-color:var(--clr-green-teal);
}

.summary__wrapper--blue {
--item-color:var(--clr-cobalt-blue);
}
```




### Useful resources

- [Kevin Powell similar challenge solution](https://www.youtube.com/watch?v=KqFAs5d3Yl8&pp=ygUda2V2aW4gcG93ZWxsIGZyb250IGVuZCBtZW50b3I%3D) - Learned how he managed the color using variable. 
- [Web Dev Simplified CSS Specificity](https://www.youtube.com/watch?v=CHyPGSpIhSs&pp=ygUPY3NzIHNwZWNpZmljaXR5) - I didn't apply specificty concept here, but along the way, I have learnt about it. 




## Acknowledgments
Kevin Powell - https://www.kevinpowell.co/
Web Dev Simplified: https://www.youtube.com/@WebDevSimplified