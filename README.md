# Frontend Mentor - Sunnyside agency landing page solution

This is a solution to the [Sunnyside agency landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/sunnyside-agency-landing-page-7yVs3B6ef). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- See hover states for all interactive elements on the page

### Screenshot

#### Screensize 1440px - Desktop

![Desktop](./images/Desktop.gif)

#### Screensize 375px - Mobile

![Mobile](./images/Mobile.gif)

### Links

- View my Solution on [Frontend Mentor]()
- View the [Live Site]()

## My process

- HTML semantics
- JavaScript
- Importing Google Fonts
- Set variables
- Reset default settings
- Styles (Mobile First)

### Built with

- Semantic HTML5 markup
- JavaScript
- SASS custom properties
- CSS Grid
- CSS Flexbox
- Mobile-first workflow
- [Google Fonts](https://fonts.google.com/) - For Fonts

### What I learned

Alt attributes (textual descriptions of images added to the HTML code that a screen reader will read to a user) and the 3 types of images:

- Decorative Image
  - An image is decorative when it doesn't provide any information or context for the user to understand the content of the page.
  - The only function of a decorative image is to enhance the appearance of the page, therefor should be given an empty alt attribute.
  - Keep in mind that an empty alt attribute is different from no alt attribute at all! When no alt attribute is provided, screen readers will read out the full filename of the image.
- Functional Image
  - An image of a logo wrapped inside a link tag is an example of a functional image, because it functions as a link to return to the homepage. In this case you can use the alternate text "Return to homepage".
- Informative Image
  - These kinds of images provide visual instructions and are useful for saving space. They can also convey emotions and thoughts. An example of an image with a visual instruction is an assembly diagram for furniture or an illustration of a phone number. In this case you can use the alternate text "assembly diagram for furniture" and “Phone number”.

I also learned about the mark tag. This tag defines text that should be marked or highlighted. I have used them for the "Learn More" links to give them the style of a highlight marker:

```html
<a href="#" class="yellow_underline"><mark class="yellow">Learn more</mark></a>
<a href="#" class="red_underline"><mark class="red">Learn more</mark></a>
```

```css
// TEXT UNDERLINE MARKER STYLE
mark {
  display: inline-block;
  line-height: 0em;
  padding: 0 0.5em 0.6em 0.5em;
  border-radius: 5px;
}

.yellow {
  background-color: $ultra_light_yellow;
  &:hover {
    background-color: pink;
  }
}

.red {
  background-color: $ultra_light_red;
}

.yellow_underline:hover mark {
  background-color: $yellow;
}

.red_underline:hover mark {
  background-color: $soft_red;
}
```

## Author

- Frontend Mentor - [@kxnzx](https://www.frontendmentor.io/profile/kxnzx)
