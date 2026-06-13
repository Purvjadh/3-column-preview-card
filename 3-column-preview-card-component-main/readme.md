# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Solution Screenshot](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Google Fonts (Big Shoulders Display + Lexend Deca)

### What I learned

**Gap vs Margin on flex children:**

I found that when `display: block` is set on flex children, the `gap` property on the parent sometimes does not apply correctly. I solved this by using `margin` on the child elements instead, which gave consistent spacing across all screen sizes.

```css
/* gap wasn't working reliably, so used margin instead */
.card__title {
    margin-top: 0.5em;
    margin-bottom: 0.5em;
}
```

**Responsive layouts across different mobile screens:**

Different phones have different viewport widths which made it tricky to get the layout looking right on all of them. I had to test and adjust my media queries carefully to handle this.

### Continued development

- CSS `clamp()` for fluid typography and spacing without extra breakpoints
- Accessibility best practices — focus states, ARIA labels
- Getting more comfortable with CSS custom properties for design tokens

### Useful resources

- [MDN — CSS clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Helped me make font sizes and padding scale smoothly across devices without needing extra breakpoints.
- [CSS Tricks — A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - A great reference whenever I needed to revisit flex alignment.

### AI Collaboration

I used Claude (Anthropic) during this project:

- **What I used it for:** Debugging CSS issues (gap not working), improving responsiveness across mobile screen sizes, and writing this README.
- **What worked well:** Getting quick explanations with code examples saved a lot of time. Claude explained why `gap` was failing and suggested using `margin` instead.
- **What didn't:** Sometimes suggestions needed small tweaks to match the exact design spec.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- GitHub - [@yourusername](https://github.com/yourusername)

## Acknowledgments

Thanks to the Frontend Mentor community for sharing solutions — looking at other approaches helped me better understand flex layout and responsive design.