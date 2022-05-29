# Frontend Mentor - Advice generator app solution

This is a solution to the [Advice generator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/advice-generator-app-QdUG-13db). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Generate a new piece of advice by clicking the dice icon

### Screenshot

![](./screenshots/desktop.png.jpg)
![](./screenshots/mobile.png.jpg)

### Links

- [Solution URL](https://github.com/wllyvx/frontendmentor-advice-generator)
- [Live Site URL](https://wllyvx.github.io/frontendmentor-advice-generator/)

## My process

### Built with
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [Tailwind CSS](https://tailwindcss.com/) - For styles

### What I learned

I learned how to consume API

```js
function onBtnClick() {
    fetch('https://api.adviceslip.com/advice', {cache: 'no-store'})
    .then(resp => resp.json())
    .then(jsonData => {
        id_tag.innerText = 'advice #' + jsonData['slip']['id'];
        advice_tag.innerText = '"' + jsonData['slip']['advice'] + '"';
    }); 
} 
```

## Author

- Willy Fajar Ramadhan
- Frontend Mentor - [@wllyvx](https://www.frontendmentor.io/profile/wllyvx)
- Github - [wllyvx](https://github.com/wllyvx)
- Twitter - [@willyframadhan](https://www.twitter.com/willyframadhan)
