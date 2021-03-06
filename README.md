## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#What-I-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](https://github.com/Just9krish/Suite-Landing-Page/blob/021f4bdfa4b73666b005f9cd960a2d0179255bf0/desktop-screenshot.png)

### Links

- Solution URL: [Click here](https://github.com/Just9krish/Suite-Landing-Page)
- Live Site URL: [Click here](https://suite-landing-page-by-just9krish.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- CSS animation

### What I learned

- Using `<picture>` element to provide "webp" format images and "2X" images for higher DPI displays.

- Use CSS Grid to make layouts with overlapping elements.

```html
<picture class="hero-img">
  <source
    srcset="
      ./assets/image-hero-portrait.webp,
      ./assets/image-hero-portrait@2x.webp 2x
    "
    type="image/webp"
    media="(min-width: 768px)"
  />
  <source
    srcset="
      ./assets/image-hero-portrait.png,
      ./assets/image-hero-portrait@2x.png 2x
    "
    type="image/png"
    media="(min-width: 768px)"
  />
  <source
    srcset="
      ./assets/image-hero-landscape.webp,
      ./assets/image-hero-landscape@2x.webp 2x
    "
    type="image/webp"
  />
  <source
    srcset="
      ./assets/image-hero-landscape.png,
      ./assets/image-hero-landscape@2x.png 2x
    "
    type="image/png"
  />
  <img
    src="./assets/image-hero-landscape.png"
    width="343"
    height="240"
    alt="Suite mobile app"
  />
</picture>
```

```css
.hero-img {
  text-align: center;
}

.hero-img img {
  width: min(100%, 28rem);
  height: auto;
}
```


## Author

- Frontend Mentor - [@Just9krish](https://www.frontendmentor.io/profile/Just9krish)
- Instagram - [@Just9krish](https://www.instagram.com/just9krish/)
- Linkedin - [@rvamit2648](https://linkedin.com/in/amit-vishwakarma-bb54b222a)
