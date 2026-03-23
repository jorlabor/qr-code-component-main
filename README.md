# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Issues and Solutions](#issues-and-solutions)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [https://github.com/jorlabor/qr-code-component](https://github.com/jorlabor/qr-code-component)
- Live Site URL: [https://jorlabor.github.io/qr-code-component/](https://jorlabor.github.io/qr-code-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (Variables)
- BEM (Block Element Modifier) methodology
- CSS Grid for layout
- Relative units (rem) for accessibility
- Mobile-first workflow

### What I learned

During this project, I focused on writing clean, maintainable, and accessible code. Here are some key takeaways:

1.  **BEM Methodology**: I learned how to structure my CSS classes to be more readable and independent of HTML tags.
    ```css
    .card__title {
      color: var(--slate-900);
      font-size: 1.375rem;
    }
    ```

2.  **Semantic HTML**: I moved beyond just using `div` tags. I learned how to use `<main>`, `<article>`, `<figure>`, and `<figcaption>` to make the content more meaningful for assistive technologies.

3.  **Relative Units**: I switched from `px` to `rem` for almost all measurements, which ensures the layout scales correctly with the user's browser settings.

### Issues and Solutions

- **Landmark Accessibility**: I initially had content floating in `div`s. I learned that every page should have a `<main>` landmark and a `<footer>` for better navigation by screen readers.
- **Image-Caption Relationship**: The QR image and its text were separate. I solved this by grouping them in a `<figure>` with a `<figcaption>`, which explicitly links the visual content to its description.
- **Concentric Corner Curves**: I struggled with making the inner image corners match the outer card corners. I learned that subtracting a small offset from the outer radius (`calc(var(--radius) - 0.375rem)`) creates a more natural, "concentric" look.

### Continued development

In future projects, I want to:
- Explore more complex CSS Grid layouts.
- Implement more advanced accessibility features like focus management.
- Start incorporating CSS `clamp()` for truly fluid typography.

### AI Collaboration

I worked with an AI pair programmer to refine my solution. 

- **Tools Used**: Trae IDE (Gemini-3-Flash).
- **Process**: The AI acted as a mentor, guiding me through refactoring to BEM, explaining accessibility concepts (like landmarks and semantic grouping), and helping me convert my fixed pixel values to relative units.
- **Outcome**: This collaboration helped me understand the "why" behind best practices, not just the "how".

## Author

- Frontend Mentor - [@jorlabor](https://www.frontendmentor.io/profile/jorlabor)
