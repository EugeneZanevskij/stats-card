# Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

Desktop version

![](screenshots/screen-desktop.png)

[Mobile version](screenshots/screen-mobile.png)

### Links

- Solution URL: [Stats Preview Card GitHub]()
- Live Site URL: [Stats Preview Card Live version]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- BEM
- SCSS
- npm sass

### What I learned

This was the 2 project I worked on using SCSS. It's getting easier... 

Better BEM understanding comes. Hopefully it's okay)

For `:before` element i came up with this @Mixin:

```scss
@mixin before-background($height, $width, $before) {
    height: $height;
    position: relative;
    z-index: 1;

    &:before{
        content: '';
        display: block;
        height: $height;
        position: absolute;
        top: 0;
        left: 0;
        width: $width;
        z-index: 2;
        background: $before;

        @content;
    }
}
```

When using `sass` in order to build this solution:

- Install `sass`:

```bash
npm install -g sass
```

- Run build command from command line:

```bash
sass src/sass/main.scss src/css/main.css
```

- If you want to edit the code and test:

```bash
sass --watch sass/main.scss css/main.css
```

### Continued development

In future projects I want to focus on writing sustainable SCSS and get aquinted with BEM method. 

I want to learn how to use Gulp.

### Useful resources

- [Sass Guidelines](https://sass-guidelin.es/) - An opinionated styleguide for writing sane, maintainable and scalable Sass.
- [Sass Basics](https://sass-lang.com/guide) - Basics on how to transform SCSS into CSS using terminal.
- [BEM](https://css-tricks.com/bem-101/) - Basics of BEM methodology.

## Author

- LinkedIn - [Eugene Zanevskij](https://www.linkedin.com/in/eugene-zanevskij/)
- Frontend Mentor - [@EugeneZanevskij](https://www.frontendmentor.io/profile/EugeneZanevskij)
- GitHub - [@EugeneZanevskij](https://github.com/EugeneZanevskij)