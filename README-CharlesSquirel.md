# Frontend Mentor - NFT preview card component solution

My third project with frontendmentor.io and third project ever.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

/screenshot.jpg

### Links

- Solution URL: https://github.com/CharlesSquirel/NFT-preview-card-component
- Live Site URL: https://nft-preview-card-component-m37o.vercel.app/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

1. I learned how to hover img with using overlay method with opacity properties and position absolute:

```css
.hover {
  display: block;
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  width: 278px;
  height: 278px;
  top: 54%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.overlay {
  position: relative;
}

.overlay:hover .cube {
  opacity: 1;
}

.overlay:hover .hover {
  opacity: 0.5;
  cursor: pointer;
  background: #00FFF8;
  mix-blend-mode: normal;
  display: block;
}

#eye {
  display: block;
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  top: 54%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.overlay:hover #eye {
  opacity: 1;
}
```
2. I was a problem with styling span element with „Jules Wyvern”. The white color didn't appear, when I set „color: #ffffff;”.

### Useful resources

- https://www.w3schools.com/howto/howto_css_image_overlay.asp - This helped me for overlay hover with opacity properties and position absolute.

## Author

- Frontend Mentor - @CharlesSquirel
- GitHub - CharlesSquirel

## Acknowledgments

From @correlucas:
1. I should not have used fixed width value on the container's divs, for better RWD.
2. I should avoid hover effects that provide touch on mobile with such kind a code:
```css
@media (hover: hover) {
{ADD HERE ALL THE CLASSES WITH HOVER EFFECTS TO DISABLE IT ON MOBILE}
}
```
