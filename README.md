# Random-choice-picker

This is apart of the 50 projects in 50 days challenge and is the thirteenth project.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

- To create a random choice picker that randomly picks an option that you wrote. The challenge involves HTML, CSS and Javascript.

### Screenshot

# Mobile Preview 

![screenshot](https://github.com/romila2003/Random-choice-picker/blob/main/Mobile%20preview.PNG)

# Mobile Preview - active

![screenshot](https://github.com/romila2003/Random-choice-picker/blob/main/Mobile%20preview%20-%20active.PNG)

# Desktop Preview 

![screenshot](https://github.com/romila2003/Random-choice-picker/blob/main/Desktop%20preview.PNG)

# Desktop Preview - active

![screenshot](https://github.com/romila2003/Random-choice-picker/blob/main/Desktop%20preview%20-%20active.PNG)


### Links

 - Source code: [https://github.com/romila2003/Random-choice-picker](https://github.com/romila2003/Random-choice-picker)
 - Live website: [https://random-choice-picker-main.netlify.app/](https://random-choice-picker-main.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- Plain CSS
- Vanilla Javascript
- Flexbox

### What I learned

This project helped me to learn concepts about setting a Timeout so that the random choice will land on one of the choices.

Javascript - `setTimeOut()` and `randomSelect()`:

```javascript

function randomSelect() {
    const times = 30;
    const int = 100;

    const interval = setInterval(() => {
        const randomTag = pickRandomTag();

        highlightTag(randomTag);

        setTimeout(() => {
            unhighlightTag(randomTag);
        }, int);

    }, int);

    setTimeout(() => {
        clearInterval(interval);

        setTimeout(() => {
            const randomTag = pickRandomTag();

            highlightTag(randomTag);
        });
    }, int * times);
}

```

### Continued development

I'll try to continue to complete 1 project a day, to learn new javascript concepts so that I can practice it on challenges in frontendmentor.io.


## Author

- Twitter - [@romila003](https://www.twitter.com/romila003)
- Frontend Mentor - [@romila2003](https://www.frontendmentor.io/profile/romila2003)
