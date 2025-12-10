# Frontend Mentor - FAQ accordion solution

This is a solution to the [FAQ accordion challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- Hide/Show the answer to a question when the question is clicked
- Navigate the questions and hide/show answers using keyboard navigation alone
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

```html
<!-- NATIVE HTML ACCORDION -->
<details open>
    <summary><h2>What is Frontend Mentor, and how will it help me?</h2></summary>
    <p>Frontend Mentor offers realistic coding challenges to help developers improve their frontend coding skills with projects in HTML, CSS, and JavaScript. It's suitable for all levels and ideal for portfolio building.</p>
</details>
```
```css
/* disable ::marker */

summary {
  list-style: none;
}

summary::-webkit-details-marker {
    display: none;
}

/* add custom marker */
summary::after {
    content: url('./assets/images/icon-plus.svg');
    cursor: pointer;
}

/* on open, change custom marker */
details[open] summary::after,
details:open summary::after {
    content: url('./assets/images/icon-minus.svg');
}
```

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/ashkir004)

## Acknowledgements

- [Frontendmentor.io](https://www.frontendmentor.io)
- [Netlify.com](https://www.netlify.com)