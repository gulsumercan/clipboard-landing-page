# Frontend Mentor - Clipboard landing page solution

This is a solution to the [Clipboard landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/clipboard-landing-page-91oN7q7A7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![Desktop Preview](/images/desktop.png)

### Links

https://grand-twilight-fec50e.netlify.app/

## My process

1. **Desktop Architecture:** First, I built the foundational layout for the desktop view, creating reusable component classes for buttons and highly flexible row/column classes using a CSS Grid and Flexbox hybrid structure.
2. **Interactive States & Accessibility:** Next, I implemented smooth hover effects and strict keyboard navigation controls using `:focus-visible` to ensure distinct, accessible focus rings across all active elements.
3. **Responsive Breakpoints:** Finally, I configured optimized media queries below the 850px breakpoint to transform the layout into a perfectly adaptive mobile-responsive experience.

### Built with

- Semantic HTML5 markup
- CSS Custom Properties (Variables)
- Flexbox
- CSS Grid
- Mobile-first workflow
- WCAG Accessibility standards (ARIA labels & Focus indicators)

### What I learned

During this project, I focused heavily on web accessibility (WCAG) and layouts. I learned how to handle custom focus rings cleanly using `:focus-visible` and how to correctly apply `aria-hidden="true"` and `aria-label` properties to create a seamless experience for screen reader users.

```css
.footer-socials a:focus-visible {
    outline: 2px solid var(--green-500);
    outline-offset: 2px;
    border-radius: 50%;
}
